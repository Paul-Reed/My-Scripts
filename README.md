## MQTT-Daemon

This is a init file to start/stop/restart the phpmqtt.php script, which is required to enable emonmcms to subscribe to MQTT topics.

####Obtain the init script

    cd /home/pi
    git clone https://github.com/Paul-Reed/emoncms-MQTT-Daemon.git
    cp emoncms-MQTT-Daemon/phpmqtt_input /etc/init.d/
    rm-rf emoncms-MQTT-Daemon

#### Installation

1. $ sudo chown root:root /etc/init.d/phpmqtt_input
2. $ sudo chmod +x /etc/init.d/phpmqtt_input
3. $ sudo update-rc.d phpmqtt_input defaults

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
