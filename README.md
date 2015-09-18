## MQTT-Daemon

This is a init file to start/stop/restart the phpmqtt.php script, which is required to enable emonmcms to subscribe to MQTT topics.

#### Installation

1. Move this file to the /etc/init.d/ folder
2. $ sudo chown root:root /etc/init.d/phpmqtt_input
3. $ sudo chmod +x /etc/init.d/phpmqtt_input
4. $ sudo update-rc.d phpmqtt_input defaults

#### Starting and stopping

Start:

    $ sudo service phpmqtt_input start
    
or

    $ sudo /etc/init.d/phpmqtt_input start
    
Stop:

    $ sudo service phpmqtt_input stop
    
or

    $ sudo /etc/init.d/phpmqtt_input stop
    
Show process ID:

    $ cat /var/run/phpmqtt_input.pid
