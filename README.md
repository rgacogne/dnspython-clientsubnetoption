# ClientSubnetOption

Class to add [draft-vandergaast-edns-client-subnet-01](http://tools.ietf.org/html/draft-vandergaast-edns-client-subnet-01) support to [dnspython](http://www.dnspython.org).

## Installation

`pip install clientsubnetoption`

## Requirements

* [python](http://www.python.org) 2.7 or later
* [dnspython](http://www.dnspython.org) 1.10.0 or later

**Note**: If you are installing dnspython on Python3, use `pip install dnspython3`

## Changelog

### 2.0.0
 * Python 3 compatible (tested with 3.4.3 & 2.7.10)
 * Can be installed via pip: `pip install clientsubnetoption`
 * Family is now auto-detected
 * IPs must be given as strings (versus their unpacked form)
  * `ClientSubnetOption('192.168.1.1')` vs `ClientSubnetOption(struct.unpack('!L', socket.inet_aton('192.168.1.1'))[0])`
