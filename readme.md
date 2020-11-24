# Awesome WebDAV [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of awesome apps that support the WebDAV protocol ([RFC 4918](https://tools.ietf.org/html/rfc4918)) and tools related to it.

Inspired by the [awesome](https://github.com/sindresorhus/awesome) list thing. Feel free to improve this list by [contributing](contributing.md)!

## Table of Contents
- [Resources](#resources)
  - [General](#general)
  - [Client guides](#client-guides)
  - [Server guides](#server-guides)
- [Servers](#servers)
  - [Standalone](#standalone)
  - [Web servers](#web-servers)
  - [Docker images](#docker-images)
- [Desktop apps](#desktop-apps)
  - [File managers](#desktop-file-managers)
  - [Other apps](#desktop-other-apps)
- [Mobile apps](#mobile-apps)
  - [Android](#android)
    - [File managers](#android-file-managers)
    - [Other apps](#android-other-apps)
  - [iOS](#ios)
    - [File managers](#ios-file-managers)
  - [Cloud providers](#cloud-providers)
  - [Extensions](#extensions)

## Resources

### General

*General information about WebDAV*

- [Wikipedia article](https://en.wikipedia.org/wiki/WebDAV)
- [DAV Frequently Asked Questions](http://www.webdav.org/other/faq.html)

### Client guides

*Mounting a WebDAV volume if you have an existing server*

- [Connect to or disconnect from a WebDAV server on Mac](https://support.apple.com/en-au/guide/mac-help/mchlp1546/mac)
- [Accessing WebDAV with Windows](https://help.dreamhost.com/hc/en-us/articles/216473357-Accessing-WebDAV-with-Windows)
- [How do I establish a WebDAV connection in Gnome 3?](https://askubuntu.com/questions/233242/how-do-i-establish-a-webdav-connection-in-gnome-3)

### Server guides

*Setting up a WebDAV server*

- [How To Configure WebDAV Access with Apache on Ubuntu 14.04](https://www.digitalocean.com/community/tutorials/how-to-configure-webdav-access-with-apache-on-ubuntu-14-04)
- [Run your own WebDAV server with Docker](https://docs.bytemark.co.uk/article/run-your-own-webdav-server-with-docker/)

## Servers

### Standalone

*Standalone servers specifically built for WebDAV and its extensions*

- [sabre/dav](https://sabre.io/)

### Web servers

*Web servers that support WebDAV or have modules to enable WebDAV support*

- [Apache HTTP Server](https://httpd.apache.org/docs/2.4/mod/mod_dav.html) supports WebDAV via the `mod_dav` module
- [Caddy](https://caddyserver.com/docs/modules/http.handlers.webdav) supports WebDAV via the `http.handlers.webdav` module
- [lighttpd](https://redmine.lighttpd.net/projects/1/wiki/Docs_ModWebDAV) supports WebDAV via the `mod_webdav` module
- [Microsoft Internet Information Services (IIS)](https://docs.microsoft.com/en-us/iis/configuration/system.webServer/webdav/) supports WebDAV starting with version 7.0 when *WebDAV Publishing* is enabled
- [nginx](https://nginx.org/en/docs/http/ngx_http_dav_module.html) supports a subset of WebDAV methods via the `ngx_http_dav_module` module
  - [`nginx-dav-ext-module`](https://github.com/arut/nginx-dav-ext-module) is an unofficial module that adds full WebDAV support

### Docker images

*Docker images for easily deploying a WebDAV server*

- [bytemark/webdav](https://hub.docker.com/r/bytemark/webdav) - based on Apache HTTP Server
- [ugeek/webdav](https://hub.docker.com/r/ugeek/webdav) - based on nginx

## Desktop apps

<a name="desktop-file-managers" />

### File managers

*General purpose apps to browse and manage files on a WebDAV server*

- [FileZilla Pro](https://filezillapro.com/how-to-connect-to-webdav/) - file transfer tool that supports many protocols, including WebDAV (for Windows, Mac and Linux)
- [WinSCP](https://winscp.net/eng/docs/webdav) - popular SFTP client that also supports WebDAV (for Windows)
- [davfs2](https://savannah.nongnu.org/projects/davfs2) - allows mounting a WebDAV server as a local filesystem (for Linux)

<a name="desktop-other-apps" />

### Other apps

*Apps and browser extensions that support WebDAV in some form, e.g. for backup and sync*

- [KeePass Password Safe](https://keepass.info/) - password manager that supports WebDAV sync (for Windows)
- [floccus](https://floccus.org/) - browser extension for bookmark sync that supports WebDAV (for Chrome, Firefox and Edge)

## Mobile apps

### Android

<a name="android-file-managers" />

#### File managers

*General purpose apps to browse and manage files on a WebDAV server*

- [WebDAV Navigator](https://play.google.com/store/apps/details?id=com.schimera.webdavnav) - WebDAV client for Android devices
- [Total Commander](https://play.google.com/store/apps/details?id=com.ghisler.android.TotalCommander) - file manager that has a WebDAV plugin

<a name="android-other-apps" />

#### Other apps

*Apps that support WebDAV in some form, e.g. for backup and sync*

- [Joplin](https://play.google.com/store/apps/details?id=net.cozic.joplin) - note taking and to-do application that supports WebDAV sync
- [Keepass2Android](https://play.google.com/store/apps/details?id=keepass2android.keepass2android) - password manager that supports WebDAV sync

### iOS

<a name="ios-file-managers" />

#### File managers

*General purpose apps to browse and manage files on a WebDAV server*

- [WebDAV Navigator](https://apps.apple.com/gb/app/webdav-navigator/id382551345) - download, share, store and edit files on a WebDAV server

## Cloud providers

*Cloud services that offer a WebDAV server or otherwise allow access via WebDAV*

- [Nextcloud](https://docs.nextcloud.com/server/latest/user_manual/en/files/access_webdav.html) fully supports WebDAV and allows synchronization over it
- [ownCloud](https://doc.owncloud.org/server/latest/user_manual/files/access_webdav.html) fully supports WebDAV and allows synchronization over it
- [Yandex.Disk](https://yandex.com/dev/disk/webdav/) has a WebDAV API that treats its storage like a file system
- [~~Box~~](https://support.box.com/hc/en-us/articles/360043696414-WebDAV-with-Box) has a WebDAV URL that allows access via WebDAV (no longer supported)

## Extensions

*Protocol extensions and related protocols*

- [CalDAV](https://en.wikipedia.org/wiki/CalDAV)
- [CardDAV](https://en.wikipedia.org/wiki/CardDAV)
- [GroupDAV](https://en.wikipedia.org/wiki/GroupDAV)
- [Microsoft Extensions](https://docs.microsoft.com/en-us/openspecs/sharepoint_protocols/ms-wdvme/8cafdf55-ee5c-443e-bdb7-2cb2ab1fb2c3)

## Contribute

Contributions welcome! Read the [contribution guidelines](contributing.md) first.

## License

[![CC0](http://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0/)
