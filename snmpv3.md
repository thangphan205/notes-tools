# SNMPv3 configuration

## Ubuntu

## Cisco IOS

## Cisco Nexus
```
snmp-server user <user> auth sha <password> priv aes-128 <secret>
snmp-server user monitor auth sha xxx.2020 priv aes-128 yyy.2020
```
## Juniper

## Aruba

## check snmp: snmpwalk1
```
snmpwalk -v3 -l authPriv -u <user> -a SHA -A <password> -x AES -X <secret> <hostname/IP>
snmpwalk -v3 -l authPriv -u monitor -a SHA -A xxx.2020 -x AES -X yyy.2020 11.0.0.1
```