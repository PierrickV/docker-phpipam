![phpipam](https://raw.githubusercontent.com/PierrickV/phpipam/master/images/logo.png "Phpipam.net logo")

# Docker image for phpIPAM

## How to use

```
git clone https://github.com/Newlode/phpipam.git
sudo docker-compose up
```

## Features
* Based on [debian/stretch](https://hub.docker.com/_/debian/)
* phpipam auto-installation
* ~~Support of of [Kea-1.1.0-beta](http://kea.isc.org/wiki) (DHCP)~~ - [Not working yet](https://github.com/phpipam/phpipam/issues/777)
* Support of [PowerDNS](https://www.powerdns.com/)
* Support of SNMP

## Roadmap
* Make the PROXY_ variables work
* Add phpipam-agent support
* Add "[Crons for phpIPAM ping check, DNS resolution and host discovery](https://github.com/phpipam/phpipam/issues/762)"
* See if patch from [fanfoni/phpipam](https://bitbucket.org/thiagofanfoni/phpipam/commits/4a96bc18b6b337e1cbffff9794a515e6b72eb780?at=master) is needed

## Misc

### Default login:
admin / ipamadmin

### PowerDns configuration exemple:
![PowerDns configuration Example](https://raw.githubusercontent.com/PierrickV/phpipam/master/images/powerdns_conf.png)

## Variable list

| Variable         | Values        | Default |
| :----------------|:-------------:|--------:|
| DEBUG            | true or false | false   |
| PROXY_ENABLED    | true or false | false   |
| PROXY_ADDRESS    | any           | emtpy   |
| PROXY_PORT       | any           | empty   |
| PROXY_AUTH       | true or false | false   |
| PROXY_USER       | any           | empty   |
| PROXY_PASSWORD   | any           | empty   |
| SSL_OFFLOAD      | true or false | false   |
| DATABASE_HOST    | any           | empty   |
| DATABASE_PORT    | any           | 3306    |
| DATABASE_NAME     | any           | empty   |
| DATABASE_USER    | any           | root    |
| DATABASE_PASSWORD | any           | empty   |

## Sources

* [RafPe/docker-phpipam](https://github.com/RafPe/docker-phpipam)
* [fanfoni/phpipam](https://bitbucket.org/thiagofanfoni/phpipam)
* [pierrecdn/phpipam](https://github.com/pierrecdn/phpipam)
* [mrlesmithjr/docker-phpipam](mrlesmithjr/docker-phpipam)
* [phpipam.net](http://phpipam.net)
