# Linux Server Configuration

### Server Details
* Instance: `Ubuntu 16.04 LTS`
* Public IP Address: `34.234.100.0`
* SSH Port: `2200`

### Web App URLs
* Portfolio Webpage: <http://spencereick.aevasun.com>
* Venue Catalog: <http://venuecatalog.aevasun.com>
* Neighborhood Map: <http://neighborhoodmap.aevasun.com>

### Installed Software
* finger
* pip3
* flask
* apache2
* libapache2-mod-wsgi-py3
* postgresql
* git
* sqlalchemy
* oauth2client
* datetime

### Security/Configuration
* All base install packages have been upgraded
* Remote login of root user disabled
* Default SSH port changed to `2200`
* Firewall accepts connections from only ports `80` (HTTP), `123` (NTP), and
`2200` (the custom SSH port)
* Key-based authentication is enforced
* Local timezone set to UTC
* Remote connections disabled for PostgreSQL
* Webserver configured to host the Venue Catalog app as a WSGI application

### Reference Material
* http://terokarvinen.com/2016/deploy-flask-python3-on-apache2-ubuntu
* https://help.ubuntu.com/community/PostgreSQL
* http://modwsgi.readthedocs.io/en/develop/user-guides/quick-configuration-guide.html
* https://help.ubuntu.com/community/PostgreSQL#Basic_Server_Setup
* http://docs.sqlalchemy.org/en/latest/core/engines.html#postgresql
* https://www.postgresql.org/docs/9.4/static/app-psql.html
* https://www.liberiangeek.net/2014/09/run-multiple-websites-single-ubuntu-server-using-apache2
