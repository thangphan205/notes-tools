# SNMPv3 configuration

## Ubuntu
sudo apt-get -y install snmp snmpd libsnmp-dev
sudo service snmpd stop
sudo net-snmp-config --create-snmpv3-user SNMPV3USER -ro -a SHA -A AUTH-PASS -x AES -X ENCRYPT-PASS 
service snmpd start

## CentOS
yum install net-snmp
net-snmp-create-v3-user -ro -A AUTH-PASS -X ENCRYPT-PASS -a MD5 -x AES SNMPV3USER
service snmpd start

## Cisco IOS

## Cisco Nexus
```
snmp-server user SNMPV3USER auth sha AUTH-PASS priv aes-128 ENCRYPT-PASS
```
## Juniper

## Aruba

## check snmp: snmpwalk1
```
snmpwalk -v3 -l authPriv -u SNMPV3USER -a SHA -A AUTH-PASS -x AES -X ENCRYPT-PASS <hostname/IP>
```