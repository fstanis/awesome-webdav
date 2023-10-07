# Awesome WebDAV [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of awesome apps that support the WebDAV protocol ([RFC 4918](https://tools.ietf.org/html/rfc4918)) and tools related to it.

## Contents

- [Resources](#resources)
  - [General](#general)
  - [Client guides](#client-guides)
  - [Server guides](#server-guides)
- [Servers](#servers)
  - [Standalone](#standalone)
  - [Web servers](#web-servers)
  - [Docker images](#docker-images)
- [Desktop apps](#desktop-apps)
  - [File managers and tools](#file-managers-and-tools)
  - [Backup and sync](#backup-and-sync)
  - [Other apps](#other-apps)
- [Mobile apps](#mobile-apps)
  - [Android](#android)
  - [iOS](#ios)
- [Libraries](#libraries)
  - [C](#c)
  - [C++](#c-1)
  - [Go](#go)
  - [Java](#java)
  - [JavaScript](#javascript)
  - [Python](#python)
- [Cloud providers](#cloud-providers)
- [Extensions](#extensions)

## Resources

### General

_General information about WebDAV_

- [Wikipedia article](https://en.wikipedia.org/wiki/WebDAV)
- [DAV Frequently Asked Questions](http://www.webdav.org/other/faq.html)

### Client guides

_Mounting a WebDAV volume if you have an existing server_

- [Connect to or disconnect from a WebDAV server on Mac](https://support.apple.com/en-au/guide/mac-help/mchlp1546/mac)
- [Accessing WebDAV with Windows](https://help.dreamhost.com/hc/en-us/articles/216473357-Accessing-WebDAV-with-Windows)
- [How do I establish a WebDAV connection in Gnome 3?](https://askubuntu.com/questions/233242/how-do-i-establish-a-webdav-connection-in-gnome-3)

### Server guides

_Setting up a WebDAV server_

- [How To Configure WebDAV Access with Apache on Ubuntu 14.04](https://www.digitalocean.com/community/tutorials/how-to-configure-webdav-access-with-apache-on-ubuntu-14-04)
- [Run your own WebDAV server with Docker](https://docs.bytemark.co.uk/article/run-your-own-webdav-server-with-docker/)

## Servers

### Standalone

_Standalone servers specifically built for WebDAV and its extensions_

- [phởdav (a.k.a. chezdav)](https://wiki.gnome.org/phodav) - A minimal open source WebDAV server, ideal for sharing one folder (for FreeBSD, Linux, and Windows).
- [hacdias-webdav](https://github.com/hacdias/webdav) - A simple yet configurable WebDAV server written in Go.
- [sabre/dav](https://sabre.io/) - Open source CardDAV, CalDAV and WebDAV server.
- [SFTPGo](https://github.com/drakkan/sftpgo) - SFTP server with optional FTP/S and WebDAV support.

### Web servers

_Web servers that support WebDAV or have modules to enable WebDAV support_

- [Apache HTTP Server](https://httpd.apache.org/docs/2.4/mod/mod_dav.html) - Supports WebDAV via the `mod_dav` module.
- [Caddy](https://caddyserver.com/docs/modules/http.handlers.webdav) - Supports WebDAV via the `http.handlers.webdav` module.
- [lighttpd](https://redmine.lighttpd.net/projects/1/wiki/Docs_ModWebDAV) - Supports WebDAV via the `mod_webdav` module.
- [Microsoft Internet Information Services (IIS)](https://docs.microsoft.com/en-us/iis/configuration/system.webServer/webdav/) - Supports WebDAV starting with version 7.0 when _WebDAV Publishing_ is enabled.
- [nginx](https://nginx.org/en/docs/http/ngx_http_dav_module.html) - Supports a subset of WebDAV methods via the `ngx_http_dav_module` module.
  - [`nginx-dav-ext-module`](https://github.com/arut/nginx-dav-ext-module) - Unofficial module that adds full WebDAV support.

### Docker images

_Docker images for easily deploying a WebDAV server_

- [bytemark/webdav](https://hub.docker.com/r/bytemark/webdav) - Based on Apache HTTP Server.
- [ugeek/webdav](https://hub.docker.com/r/ugeek/webdav) - Based on nginx.

## Desktop apps

<a name="desktop-file-managers" />

### File managers and tools

_General purpose apps to browse and manage files on a WebDAV server_

- [Cyberduck](https://cyberduck.io/) - Libre server and cloud storage browser with WebDAV support (for Windows and Mac).
- [Mountain Duck](https://mountainduck.io/) - Lets you mount server and cloud storage including WebDAV as a disk (for Windows and Mac).
- [FileZilla Pro](https://filezillapro.com/how-to-connect-to-webdav/) - File transfer tool that supports many protocols, including WebDAV (for Windows, Mac and Linux).
- [WinSCP](https://winscp.net/eng/docs/webdav) - Popular SFTP client that also supports WebDAV (for Windows).
- [davfs2](https://savannah.nongnu.org/projects/davfs2) - Allows mounting a WebDAV server as a local filesystem (for Linux).
- [CrossFTP](https://www.crossftp.com/) - Free client software that supports many protocols, including WebDAV (for Windows, Mac and Linux).
- [FileZilla Pro](https://filezillapro.com/) - Paid version of the popular FTP client includes WebDAV support (for Windows, Mac and Linux).

<a name="desktop-other-apps" />

### Backup and sync

_Apps used for backup and/or synchronizing data between multiple destinations_

- [rclone](https://rclone.org/) - Supports WebDAV as a backup target and [can itself act as a WebDAV server](https://rclone.org/commands/rclone_serve_webdav/) (for Windows, Mac and Linux).
- [Duplicacy](https://duplicacy.com/) - Beta support for WebDAV as a backup target (for Windows, Mac and Linux).
- [Duplicati](https://github.com/duplicati/duplicati) - Supports WebDAV as a backup target (for Windows, Mac and Linux).

### Other apps

_Apps and browser extensions that support WebDAV in some form, e.g. for backup and sync_

- [KeePass Password Safe](https://keepass.info/) - Password manager that supports WebDAV sync (for Windows).
- [floccus](https://floccus.org/) - Browser extension for bookmark sync that supports WebDAV (for Chrome, Firefox and Edge).
- [Stylus](https://add0n.com/stylus.html) - Browser extension for custom css that can sync with WebDAV.
- [Violentmonkey](https://violentmonkey.github.io/) - A web browser extension for UserJS management that can sync with WebDAV.

## Mobile apps

### Android

<a name="android-file-managers" />

#### File managers

_General purpose apps to browse and manage files on a WebDAV server_

- [WebDAV Navigator](https://play.google.com/store/apps/details?id=com.schimera.webdavnav) - WebDAV client for Android devices.
- [Total Commander](https://play.google.com/store/apps/details?id=com.ghisler.android.TotalCommander) - File manager that has a WebDAV plugin.
- [X-plore File Manager](https://play.google.com/store/apps/details?id=com.lonelycatgames.Xplore) - File manager supporting WebDAV mounts.
- [MiXplorer](https://forum.xda-developers.com/showpost.php?p=23109280&postcount=2) - File manager that supports WebDAV.

<a name="android-other-apps" />

#### Other apps

_Apps that support WebDAV in some form, e.g. for backup and sync_

- [Joplin](https://play.google.com/store/apps/details?id=net.cozic.joplin) - Note taking and to-do application that supports WebDAV sync.
- [Keepass2Android](https://play.google.com/store/apps/details?id=keepass2android.keepass2android) - KeePass-based password manager that supports WebDAV sync.

### iOS

<a name="ios-file-managers" />

#### File managers

_General purpose apps to browse and manage files on a WebDAV server_

- [WebDAV Nav+](https://apps.apple.com/app/webdav-nav/id412341302) - Download, share, store and edit files on a WebDAV server.
- [WebDAV Navigator](https://apps.apple.com/app/webdav-navigator/id382551345) - Download, share, store and edit files on a WebDAV server.

<a name="ios-other-apps" />

#### Other apps

_Apps that support WebDAV in some form, e.g. for backup and sync_

- [1Writer](https://apps.apple.com/app/1writer-markdown-text-editor/id680469088) - Markdown text editor that supports importing from WebDAV.
- [beorg](https://apps.apple.com/app/beorg-to-do-list-agenda/id1238649962) - TO-DO list and agenda app with WebDAV sync support.
- [GoodReader](https://apps.apple.com/app/goodreader-pdf-editor-viewer/id777310222) - PDF viewer and editor that supports WebDAV sync.
- [Joplin](https://apps.apple.com/app/joplin/id1315599797) - Note taking and to-do application that supports WebDAV sync.
- [Notebooks 10](https://apps.apple.com/app/notebooks-write-and-organize/id1490084838) - Writing app, a text and markdown editor with WebDAV support.
- [Strongbox](https://apps.apple.com/app/strongbox-password-safe/id897283731) - KeePass-based password manager that supports WebDAV sync.
- [Notability](https://apps.apple.com/app/notability/id360593530) - Note-taking app that supports webDAV for backups.

## Libraries

_Libraries for accessing a WebDAV storage and/or building a WebDAV server_

### C

- [neon](https://github.com/notroj/neon) - An HTTP/1.1 and WebDAV client library with a C API.

### C++

- [webdav-client-cpp](https://github.com/CloudPolis/webdav-client-cpp) - C++ WebDAV Client.

### Go

- [golang.org/x/net/webdav](https://godoc.org/golang.org/x/net/webdav) - WebDAV server implementation as part of the standard library.
- [go-webdav](https://github.com/emersion/go-webdav) - Client library for WebDAV, CalDAV and CardDAV.
- [gowebdav](https://github.com/studio-b12/gowebdav) - WebDAV client library and command line tool.

### Java

- [Jackrabbit WebDAV Library](https://jackrabbit.apache.org/jcr/components/jackrabbit-webdav-library.html) - WebDAV Library component of the Apache Jackrabbit project.

### JavaScript

- [webdav](https://github.com/perry-mitchell/webdav-client) - WebDAV client written in JavaScript for Node.js and the browser.
- [unifile](https://github.com/silexlabs/unifile) - Node.js library to access cloud storage which supports WebDAV.

### Python

- [webdavclient3](https://pypi.org/project/webdavclient3/) - WebDAV client for Python 3.x.

## Cloud providers

_Cloud services that offer a WebDAV server or otherwise allow access via WebDAV_

- [4shared](https://www.4shared.com/web/helpCenter/fGeDNHCrXce#par_eight) - Fully supports WebDAV and allows synchronization over it.
- [Nextcloud](https://docs.nextcloud.com/server/latest/user_manual/en/files/access_webdav.html) - Fully supports WebDAV and allows synchronization over it.
- [ownCloud](https://doc.owncloud.org/server/latest/user_manual/files/access_webdav.html) - Fully supports WebDAV and allows synchronization over it.
- [Yandex.Disk](https://yandex.com/dev/disk/webdav/) - Has a WebDAV API that treats its storage like a file system.
- [~Box~](https://support.box.com/hc/en-us/articles/360043696414-WebDAV-with-Box) - Has a WebDAV URL that allows access via WebDAV (no longer supported).

## Extensions

_Protocol extensions and related protocols_

- [CalDAV](https://en.wikipedia.org/wiki/CalDAV)
- [CardDAV](https://en.wikipedia.org/wiki/CardDAV)
- [GroupDAV](https://en.wikipedia.org/wiki/GroupDAV)
- [Microsoft Extensions](https://docs.microsoft.com/en-us/openspecs/sharepoint_protocols/ms-wdvme/8cafdf55-ee5c-443e-bdb7-2cb2ab1fb2c3)

## Contributing

Contributions welcome! Read the [contribution guidelines](contributing.md) first.
