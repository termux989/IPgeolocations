A tool to retrieve IP geolocations information
Powered by ip-api
Requirements

Python 3.x
termcolor
colorama
Download/Installation

git clone https://github.com/termux989/IPgeolocations.git

pip3 install -r requirements.txt --user
if pip3 is missing:

apt-get install python3-setuptools
easy_install3 pip
pip3 install -r requirements.txt
Features

Retrieve IP or Domain Geolocation.
Retrieve your own IP Geolocation.
Retrieve Geolocation for IPs or Domains loaded from file. Each target in new line.
Define your own custom User Agent string.
Select random User-Agent strings from file. Each User Agent string in new line.
Proxy support.
Select random proxy from file. Each proxy URL in new line.
Open IP geolocation in Google Maps using the default browser.
Export results to csv, xml and txt format.
Geolocation Information

ASN
City
Country
Country Code
ISP
Latitude
Longtitude
Organization
Region Code
Region Name
Timezone
Zip CodeRetrieve your IP Geolocation

./ip2geolocation.py -m
Retrieve IP Geolocation

./ip2geolocation.py -t x.x.x.x
Retrieve Domain Geolocation

./ip2geolocation.py -t example.com
Do not save .log files

./ip2geolocation.py -t example.com --nolog
Custom User Agent string

./ip2geolocation.py -t x.x.x.x -u "Mozilla/5.0 (Windows NT 6.3; WOW64; Trident/7.0; rv:11.0) like Gecko"
Using Proxy

./ip2geolocation.py -t x.x.x.x -x http://127.0.0.1:8080
Using random Proxy

./ip2geolocation.py -t x.x.x.x -X /path/to/proxies/filename.txt
Pick User-Agent string randomly

./ip2geolocation.py -t x.x.x.x -U /path/to/user/agent/strings/filename.txt
Retrieve IP geolocation and open location in Google maps with default browser

./ip2geolocation.py -t x.x.x.x -g
Export results to CSV file

./ip2geolocation.py -t x.x.x.x --csv /path/to/results.csv
Export results to XML file

./ip2geolocation.py -t x.x.x.x --xml /path/to/results.xml
Export results to TXT file

./ip2geolocation.py -t x.x.x.x -e /path/to/results.txt
Retrieve IP Geolocation for many targets

./ip2geolocation.py -T /path/to/targets/targets.txt
Retrieve IP Geolocation for many targets and export results to xml

./ip2geolocation.py -T /path/to/targets/targets.txt --xml /path/to/results.xml
Do not print results to terminal

./ip2geolocation.py -m -e /path/to/results.txt --noprint

