# pimote
Simple Python scripts to turn on/off Pi-mote by Energenie sockets. Requires Python 2.7.

Based on Energenie's default Python scripts - just created individual Python scripts for individual activation.

Can be run via Crontab. For example:

	# Turn on Dining Room Light from Monday to Friday at 4:45pm
	45 16 * * 1-5 /usr/bin/python /home/pi/pimote/socket1-on.py

	# Turn off Dining Room Light from Monday to Friday at 7:45pm
	45 19 * * 1-5 /usr/bin/python /home/pi/pimote/socket1-off.py

	# Turn on Front Room Light from Monday to Friday at 7:20am
	20 07 * * 1-5 /usr/bin/python /home/pi/pimote/socket2-on.py

	# Turn off Front Room Light from Monday to Friday at 8:15am
	15 08 * * 1-5 /usr/bin/python /home/pi/pimote/socket2-off.py

	# Turn on Front Room Light from Monday to Friday at 5:15pm
	15 17 * * 1-5 /usr/bin/python /home/pi/pimote/socket2-on.py

	# Turn off Front Room Light from Monday to Friday at 9:00pm
	00 21 * * 1-5 /usr/bin/python /home/pi/pimote/socket2-off.py

	# Turn on Front Room Light at the Weekend at 3:30pm
	30 15 * * 6,0 /usr/bin/python /home/pi/pimote/socket2-on.py

	# Turn off Front Room Light at the Weekend at 9:15pm
	15 21 * * 6,0 /usr/bin/python /home/pi/pimote/socket2-off.py

	# Turn on Dining Room Light at the Weekend at 5:00pm
	00 17 * * 6,0 /usr/bin/python /home/pi/pimote/socket1-on.py

	# Turn off Dining Room Light at the Weekend at 7:30pm
	30 19 * * 6,0 /usr/bin/python /home/pi/pimote/socket1-off.py

This will turn lights on and off at designated times throughout the week, including a varied schedule at the weekend.