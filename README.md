# Linux Server Configuration

### Server Details
* Instance: `Ubuntu 16.04 LTS`
* IP Address: `34.234.100.0`
* SSH Port: `2200`
* Web App URL: `http://ec2-34-234-100-0.us-east-1a.compute.amazonaws.com`

### Installed Software

### Configuration
* All base install packages have been upgraded
* Default SSH port changed to `2200`
* Firewall accepts connections from only ports `80` (HTTP), `123` (NTP), and
`2200` (the custom SSH port)
