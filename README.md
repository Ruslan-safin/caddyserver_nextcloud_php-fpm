# README

## What is Nextcloud

Nextcloud is a suite of client-server software for creating and using file hosting services. It is enterprise-ready with comprehensive support options. Free and open-source means that anyone is allowed to install and operate it on their own private server devices.

Nextcloud is functionally similar to Dropbox, Office 365, or Google Drive when used with its integrated office suite solutions Collabora Online or OnlyOffice. It can be hosted in the cloud or on-premise. It is scalable from home office solutions based on the low-cost Raspberry Pi all the way through to full-sized data center solutions that support millions of users.


## What is Caddy

Caddy is a powerful, extensible platform to serve your sites, services, and apps, written in Go. Although most people use it as a web server or proxy, and operates primarily at L4 (transport layer) and L7 (application layer) of the OSI model, though it has the ability to work with other layers.


## Version 24.04.21


## How do I get set up?

1. First step - clone current repo to host
1. Change current directory to directory with downloaded files
1. Create directories: `mkdir nextcloud` and` mkdir caddy`
1. Edit Caddy config file `vi Caddyfile` or` nano Caddyfile` or `sometexeditor Caddyfile` * J *
1. Replace on Caddyfile `DOMAIL.TLD` to your domain f.e. `nextcloud.contoso.com`
1. Install docker and docker-compose
1. Run container `docker-compose -f docker-compose.yml up -d`
1.For update run `docker-compose -f docker-compose.yml pull` then` docker-compose -f docker-compose.yml down --remove-orphans` and `docker-compose -f docker-compose.yml up -d`
1. Verify service is started `docker ps -a`
1. Open service in a browser by domain name f.e. `nextcloud.contoso.com`
1. Finalize wizard and configuration steps via WebUI.

Enjoy your self-hosted file sharing service.

Who do I talk to?

Repo owner CyberManiac
