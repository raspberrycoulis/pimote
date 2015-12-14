# pimote
Simple Python scripts to turn on/off Pi-mote by Energenie sockets. Requires Python 2.7.

Based on Energenie's default Python scripts - just created individual Python scripts for individual activation.

Can be run via Crontab:

    sudo crontab -e
	30 15 * * * /usr/bin/python /home/pi/automation/lights-on.py
	15 23 * * * /usr/bin/python /home/pi/automation/lights-off.py
    Ctrl+X
