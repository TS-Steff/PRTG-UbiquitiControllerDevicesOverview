# PRTG-Ubiquiti Overview
This script gets the count of all AP's, Switches and Gateway's of the specified sites form an Ubiquiti Unifi Controller

Sensor view
![PRTG Screenshot](/Screenshots/prtg.png?raw=true "PRTG Screenshot")

The settings page may look like this
![PRTG Settings](/Screenshots/settings.png?raw=true "PRTG Sensor Settings")

## Config
Add an EXE/Script Advanced sensor to your PRTG Site

You have to pass six parameters
| parameter    | Value                                        | Comment                                                                     |
| ------------ | -------------------------------------------- | --------------------------------------------------------------------------- |
| server       | IP or hostname of your controller            | you can add %host% to for localhost                                         |
| port         | TCP port on which your cotntroller runs      |                                                                             |
| sites        | the site IDs you would like to get data from | you find the site ID in the url of each site                                |
| username     | The username to connect the controller       | this user only needs read rights on the sites defined in the sites variable |
| password     | the users password                           |                                                                             |
| debug        | debug mode                                   | writes the json to the disk if set true                                     |



## Credits
Many thants to Luciano Lingnau [Paessler Support]
- <https://kb.paessler.com/users/Luciano%20Lingnau%20%5BPaessler%20Support%5D>
- <https://kb.paessler.com/en/topic/71263-can-i-monitor-ubiquiti-unifi-network-devices-with-prtg#reply-243681>

He wrote the most part of this script. We just adopted and changed the script to fit our needs