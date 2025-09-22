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
- [PWA and online apps](#pwa)
- [Command line tools](#cli)
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
- Book [WebDAV: Next-Generation Collaborative Web Authoring: Next-Generation Collaborative Web Authoring](https://www.amazon.com/WebDAV-Next-Generation-Collaborative-Web-Authoring/dp/0130652083) - the author, goes into not only the details, but explains the problems with some of the specs (especially DeltaV).
- [Exploiting WebDAV](https://vk9-sec.com/exploiting-webdav/)
- [WebDavServer.com](https://webdavserver.com/) an online demo to test

### Client guides

_Mounting a WebDAV volume if you have an existing server_

- [Connect to or disconnect from a WebDAV server on Mac](https://support.apple.com/en-au/guide/mac-help/mchlp1546/mac)
- [Accessing WebDAV with Windows](https://help.dreamhost.com/hc/en-us/articles/216473357-Accessing-WebDAV-with-Windows)
- [How do I establish a WebDAV connection in Gnome 3?](https://askubuntu.com/questions/233242/how-do-i-establish-a-webdav-connection-in-gnome-3)

### Server guides

_Setting up a WebDAV server_

- [How To Configure WebDAV Access with Apache on Ubuntu 14.04](https://www.digitalocean.com/community/tutorials/how-to-configure-webdav-access-with-apache-on-ubuntu-14-04)
- [Run your own WebDAV server with Docker](https://docs.bytemark.co.uk/article/run-your-own-webdav-server-with-docker/)
- [WebDAV Share with Lighttpd](https://openwrt.org/docs/guide-user/services/nas/webdav) - instruction for OpenWrt WiFi routers firmware.

## Servers

### Standalone

_Standalone servers and personal cloud solutions specifically built for WebDAV and its extensions_

- [asgi-webdav](https://github.com/rexzhang/asgi-webdav) -a An asynchronous WebDAV server, Support multi-provider, multi-account and permission control. `MIT` `Python`
- [Davis](https://github.com/tchapi/davis) a simple interfacefor sabre/dav based on Symfony and Bootstrap, largely inspired by Baïkal.
- [dave](https://github.com/micromata/dave/) - a simple WebDAV server written in Go
- [FuguHub](https://fuguhub.com/) - a personal cloud server with a web ui.
- [Group-Office](https://www.group-office.com/) - Open Source CRM and Groupware with CalDAV, CardDAV and WebDAV.
- [hacdias-webdav](https://github.com/hacdias/webdav) - A simple yet configurable WebDAV server written in Go.
- [Nextcloud](https://nextcloud.com/) - Collaboration and communication platform -- includes files, calendar, contacts, mailclient, chat, videoconferencing and much more. [Try it](https://try.nextcloud.com), [Docs webDAV](https://docs.nextcloud.com/server/latest/user_manual/en/files/access_webdav.html), [Docs calDAV](https://docs.nextcloud.com/server/latest/admin_manual/groupware/calendar.html), [Docs cardDAV](https://docs.nextcloud.com/server/latest/admin_manual/groupware/contacts.html)
- [Nephele Serve](https://www.npmjs.com/package/nephele-serve) - File System or S3 Backed WebDAV Server. `Apache-2.0`
- [ownCloud](https://doc.owncloud.org/server/latest/user_manual/files/access_webdav.html) - Personal cloud solution.
- [QuickDAV](https://sciactive.com/quickdav/) - Network file transfer app. [Sources](https://github.com/sciactive/quickdav). `Apache-2.0`
- [phởdav (a.k.a. chezdav)](https://wiki.gnome.org/phodav) - A minimal open source WebDAV server, ideal for sharing one folder (for FreeBSD, Linux, and Windows).
- [miniserve](https://github.com/svenstaro/miniserve) - A file sharing server, supports read-only WebDAV
- [sabre/dav](https://sabre.io/) - Open source CardDAV, CalDAV and WebDAV server.
- [Seafile](https://github.com/haiwen/seafdav) - A webdav server written in Python
- [SFTPGo](https://github.com/drakkan/sftpgo) - SFTP server with optional FTP/S and WebDAV support.
- [Stalwart](https://github.com/stalwartlabs/stalwart) - Open-source Mailserver and WebDAV, CalDAV and CardDAV server written in Rust.
- [tolsen/limestone](https://github.com/tolsen/limestone) - Advanced WebDAV server backed by a Postgres database. Supports ACL, Search, BIND, Redirect, and partial DeltaV.
- [tolsen/limeberry](https://github.com/tolsen/limeberry) - WebDAV server (Rails 1.2)
- [weborf](https://ltworf.github.io/weborf/) - a minimal HTTP server to share your files. Has a GUI [qweborf](https://ltworf.github.io/weborf/qweborf.html).
- [WebDAV VFS gate](https://github.com/a-langer/webdav-vfs-gate) - Open source JEE application for web containers, such as Tomcat, Jetty, JBoss and similar.
- "Written in Rust". They all are similar to weborf by functionality but more advanced and fancy
  - [sigoden/dufs](https://github.com/sigoden/dufs)
  - [thecoshman/http](https://github.com/thecoshman/http)
  - [messense/dav-server-rs](https://github.com/messense/dav-server-rs) library for WebDAV and there are a lot of [small webservers based on it](https://github.com/messense/dav-server-rs/network/dependents).

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
- [stalwartlabs/stalwart](https://hub.docker.com/r/stalwartlabs/stalwart) - Open-source WebDAV, CalDAV and CardDAV server written in Rust.


<a name="pwa" />

## PWA and online apps
Online apps that can connect directly to your WebDAV share. You'll need a CORS enabled.
See an example [WebDAV with CORS using Lighttpd](https://gist.github.com/stokito/0a6274106d407ba6d9fb776e7773445d)

- [Astiga](https://asti.ga/) - an onine music player. `Proprieatary`
- [Davros](https://github.com/mnutt/davros) - a web file manager in NodeJS that uses WebDAV as a protocol. Used by [Sandstorm.io](https://sandtorm.io)
- [DevNotes](https://rainu.github.io/dev-notes/) - A notes app. [Source code](https://github.com/rainu/dev-notes)
- [Diffuse](https://diffuse.sh/) - an onine music player [Source code](https://github.com/icidasset/diffuse).
- [Filerun](https://filerun.com/) - a paid self hosted cloud. `Proprieatary`
- [Supper Productivity](https://app.super-productivity.com/) - A powerful TODO App. [Source code](https://github.com/johannesjo/super-productivity).
- [OxIDE](https://github.com/bootrino/reactoxide) - a simple code editor that you can add to your ReactJS projects. `MIT` `TypeScript`
- [TiddlyWiki](https://tiddlywiki.com/) - A non-linear notebook for capturing, organising and sharing complex information
- [KeeWeb](https://app.keeweb.info/) - A password manager [Source code](https://github.com/keeweb/keeweb)
- [webdave](https://katomaso.github.io/webdave/) - A file manager. [Source code](https://github.com/katomaso/webdave)
- [webdav-js](https://github.com/dom111/webdav-js) - A simple WebDAV file manager for use as a bookmarklet, or integration into a web server. May be used as a simplest in-browser UI
- [webdav-browser](https://github.com/WebDAVDevs/webdav-browser-extension) - a browser extension to browse a URL as a WebDAV share directly. `0BSD`, `JavaScript`

## Command line tools
<a name="cli" />

- [cadaver](https://notroj.github.io/cadaver/) - A command-line interactive FTP-like WebDAV client.
- [curl](https://gist.github.com/stokito/cf82ce965718ce87f36b78f7501d7940) - a low level command line http client that allows to query WebDAV methods.
- [davfs2](https://savannah.nongnu.org/projects/davfs2) - Allows mounting a WebDAV server as a local filesystem (for Linux).
- [DaviX](https://davix.web.cern.ch/davix/docs/devel/) - A client for WebDAV and Amazon S3 for Windows, macOS and Linux. `LGPL` `C++`
- [GNOME gvfs-mount](https://jeromebelleman.gitlab.io/posts/filesystems/gvfs/#from-a-webdav-server) - Mounting a WebDAV with GNOME Virtual Filesystem in user space. Linux.
- [KDE kioclient](https://manpages.ubuntu.com/manpages/bionic/en/man1/kioclient.1.html) - supports basic operations e.g. `kioclient cp file.txt 'webdavs://user@example.com/dav/`
- [rclone](https://rclone.org/) - Supports WebDAV as a backup target and [can itself act as a WebDAV server](https://rclone.org/commands/rclone_serve_webdav/) (for Windows, Mac and Linux).
- [litmus](https://notroj.github.io/litmus/) - a test suite from author of neon, which aims to test whether a server is compliant with the WebDAV protocol. `GPL-2.0` `C`
- [tolsen/rubydav](https://github.com/tolsen/rubydav/tree/master/test) - a test suite for WebDAV server
- [tolsen/Prestan](https://github.com/tolsen/Prestan) - a WebDAV performance benchmark
- [WebDAV-AudioPlayer](https://github.com/StefH/WebDAV-AudioPlayer) - a simple AudioPlayer (web-based Blazor & Windows WinForms).

## Desktop apps

<a name="desktop-file-managers" />

### File managers and tools

_General purpose apps to browse and manage files on a WebDAV server_

- [CrossFTP](https://www.crossftp.com/) - Free client software that supports many protocols, including WebDAV (for Windows, Mac and Linux).
- [Far Manager](https://www.farmanager.com/) - A Norton Comander like file manager for Windows. Has a NetBox plugin with WebDAV support.
- [far2l](https://github.com/elfmz/far2l) - A heavily rewritten Linux and MacOS port of FAR Manager. Has a NetRocks plugin with WebDAV support.
- [FileZilla Pro](https://filezillapro.com/how-to-connect-to-webdav/) - File transfer tool that supports many protocols, including WebDAV (for Windows, Mac and Linux).
- [SmartFTP](https://www.smartftp.com/) - A file transfer program. `Proprietary`
- [UIVI](https://sourceforge.net/projects/uivi/) - a Java GUI client. Can be runned as JNLP applet. `Public Domain` `Java`
- [WinSCP](https://winscp.net/) - A popular SFTP client that also supports WebDAV (for Windows). `Proprietary`
- [WebDrive](https://webdrive.com/) - A drive mapping utility. Windows, OS X, Android and iOS. `Proprietary`

#### macOS only
- [Commander One](https://mac.eltima.com/file-manager.html) - A file manager for macOS
- [CloudMounter](https://mac.eltima.com/mount-cloud-drive.html) - mounting cloud storages for macOS
- [Cyberduck](https://cyberduck.io/) - Libre server and cloud storage browser with WebDAV support (for Windows and Mac).
- [ForkLift](https://binarynights.com/) - A dual pane file manager and file transfer client for macOS.
- [Mountain Duck](https://mountainduck.io/) - Lets you mount server and cloud storage including WebDAV as a disk (for Windows and Mac).
- [Transmit](https://panic.com/transmit/) - A file transfer apps for macOS

<a name="desktop-other-apps" />

### Backup and sync

_Apps used for backup and/or synchronizing data between multiple destinations_

- [rclone](https://rclone.org/) - Supports WebDAV as a backup target and [can itself act as a WebDAV server](https://rclone.org/commands/rclone_serve_webdav/) (for Windows, Mac and Linux).
- [Duplicacy](https://duplicacy.com/) - Beta support for WebDAV as a backup target (for Windows, Mac and Linux).
- [Duplicati](https://github.com/duplicati/duplicati) - Supports WebDAV as a backup target (for Windows, Mac and Linux).
- [GNOME Déjà Dup](https://wiki.gnome.org/Apps/DejaDup) - Supports WebDAV as a backup target.
- [ioBroker.backitup](https://github.com/simatec/ioBroker.backitup) - a module for ioBroker home automation.

### Other apps

_Apps and browser extensions that support WebDAV in some form, e.g. for backup and sync_

- [Buttercup](https://buttercup.pw/) - A password manager. [Source code](https://github.com/buttercup)
- [Cryptomator](https://cryptomator.org/) - a tool to encrypt files and backup.
- [KODI](https://kodi.tv/) - An advanced media player for smart TV Raspberry Pi, Android, tvOS.
- [gnome-user-share](https://gitlab.gnome.org/GNOME/gnome-user-share) - configure an Apache WebDAV directly from Nautilus
- [Gnome Gnote](https://wiki.gnome.org/Apps/Gnote) - app for taking notes with WebDAV sync.
- [KeePass Password Safe](https://keepass.info/) - Password manager that supports WebDAV sync (for Windows).
- [PhotoPrism](https://photoprism.app/) AI-Powered Photos App. Supports [sync by WebDAV](https://docs.photoprism.app/user-guide/sync/webdav/)
- [Floccus](https://floccus.org/) - Browser extension for bookmark sync that supports WebDAV (for Chrome, Firefox and Edge).
- [RetroArch](https://retroarch.com) - A frontend for emulators and game engines that can use WebDAV for backing up game saves.
- [Stylus](https://add0n.com/stylus.html) - Browser extension for custom CSS that can sync with WebDAV.
- [Table Habit](https://github.com/FriesI23/mhabit) – Micro habits tracking app with [sync via WebDAV](https://github.com/FriesI23/mhabit/wiki/Feature%EA%9E%89-WebDAV-Sync). `AL2` `Dart`  `Apache-2.0`
- [Violentmonkey](https://violentmonkey.github.io/) - A web browser extension for UserJS management that can sync with WebDAV.
- [Zotero](https://www.zotero.org/) - an easy-to-use desktop app to collect, organize, annotate, cite, and share research. `AGPLv3` `JavaScript`


## Mobile apps

### Android

<a name="android-file-managers" />

#### File managers and backup

_General purpose apps to browse and manage files on a WebDAV server_

- [Android DataBackup](https://github.com/XayahSuSuSu/Android-DataBackup)
- [Cx File Explorer](https://play.google.com/store/apps/details?id=com.cxinventor.file.explorer) - File manager that has a WebDAV support built in. `Proprietary`
- [DAVx5](https://www.davx5.com/) - WebDAV, CalDAV and CardDAV client for Android.
- [EasySync](https://github.com/phpbg/easysync) - backup and sync files with WebDAV share. `MIT`
- [Total Commander](https://play.google.com/store/apps/details?id=com.ghisler.android.TotalCommander) - File manager that has a WebDAV plugin. `Proprietary`
- [X-plore File Manager](https://play.google.com/store/apps/details?id=com.lonelycatgames.Xplore) - File manager supporting WebDAV mounts. `Proprietary`
- [MiXplorer](https://forum.xda-developers.com/showpost.php?p=23109280&postcount=2) - File manager that supports WebDAV. `Proprietary`
- [FolderSync](https://play.google.com/store/apps/details?id=dk.tacit.android.foldersync.lite) - backup. `Proprietary`
- [Owlfiles](https://play.google.com/store/apps/details?id=com.skyjos.apps.fileexplorerfree) - File Manager. `Proprietary`
- [RCX](https://github.com/x0b/rcx) Rclone sync for Android (unmaintained, use Round Sync). `GPL-3.0`
- [Round Sync](https://github.com/newhinton/Round-Sync) Rclone sync for Android (fork of RCX). `GPL-3.0`
- [NextCloud Android App](https://github.com/nextcloud/android) `GPL-2.0`
- [RS File Explorer](https://play.google.com/store/apps/details?id=com.rs.explorer.filemanager) - a file manager supporting WebDAV. `Proprietary`
- [WebDAV Navigator](https://play.google.com/store/apps/details?id=com.schimera.webdavnav) - WebDAV client for Android devices. `Proprietary`
- [ndl/wedaban](https://github.com/ndl/wedaban) - an implementation of Android Backup API for backups to WebDAV servers. `WIP`
- [alexbakker/webdav-provider](https://github.com/alexbakker/webdav-provider) - WebDAV storage to other apps through Android's Storage Access Framework (SAF). `GPL-3.0`

<a name="android-players" />

#### Players

- [CloudBeats](https://www.cloudbeatsapp.com/) - A music player. `Proprietary`
- [Capriccio ](https://play.google.com/store/apps/details?id=me.ideariboso.capriccio) - a music player. `Proprietary`
- [FX Player](https://play.google.com/store/apps/details?id=tv.fipe.fplayer) - music/video player. `Proprietary`
- [GOM Player](https://play.google.com/store/apps/details?id=com.gretech.gomplayerko) - music/video player. `Proprietary`
- VLC: [is planed](https://wiki.videolan.org/Bounties/#Webdav_support)
- [danfr/webdav-player](https://github.com/danfr/webdav-player) - access to remote WebDAV repository and play media files using VLC. `WIP`
- [NOVA](https://github.com/nova-video-player/aos-AVP) - an open source video player with AndroidTV support. `Apache-2.0`
- [Neutron](https://play.google.com/store/apps/details?id=com.neutroncode.mpeval) - a music player. `Proprietary`

<a name="android-other-apps" />

#### Other apps

_Apps that support WebDAV in some form, e.g. for backup and sync_

- [Joplin](https://play.google.com/store/apps/details?id=net.cozic.joplin) - Note taking and to-do application that supports WebDAV sync.
- [Keepass2Android](https://play.google.com/store/apps/details?id=keepass2android.keepass2android) - KeePass-based password manager that supports WebDAV sync. [Sources](https://github.com/PhilippC/keepass2android). `GPL3`
- [ntodotxt](https://github.com/tmaegel/ntodotxt) - TODO App with sync via WebDAV. `MIT`
- [Orgzly](https://www.orgzly.com/) - Outliner for notes and to-do lists. [Source code](https://github.com/orgzly).
- [pokatomnik/Davno](https://github.com/pokatomnik/Davno) - webDAV NOtes. `WIP`
- [SimpleTask](https://github.com/mpcjanssen/simpletask-android) - a simple task manager. `GPL3` `Kotlin`
- [Table Habit](https://github.com/FriesI23/mhabit) – Micro habits tracking app with [sync via WebDAV](https://github.com/FriesI23/mhabit/wiki/Feature%EA%9E%89-WebDAV-Sync). `AL2` `Dart`  `Apache-2.0`


### iOS

<a name="ios-file-managers" />

#### File managers

_General purpose apps to browse and manage files on a WebDAV server_

- [Documents: File Manager & Docs](https://apps.apple.com/us/app/documents-file-manager-docs/id364901807) - PDF Converter & Reader, ZIP/RAR, suppoers WebDAV.
- [WebDAV Nav+](https://apps.apple.com/app/webdav-nav/id412341302) - Download, share, store and edit files on a WebDAV server.
- [WebDAV Navigator](https://apps.apple.com/app/webdav-navigator/id382551345) - Download, share, store and edit files on a WebDAV server.
- [Owlfiles](https://apps.apple.com/us/app/owlfiles-file-manager/id510282524) - File Manager. `Proprietary`

<a name="ios-other-apps" />

#### Other apps

_Apps that support WebDAV in some form, e.g. for backup and sync_

- [1Writer](https://apps.apple.com/app/1writer-markdown-text-editor/id680469088) - Markdown text editor that supports importing from WebDAV.
- [beorg](https://apps.apple.com/app/beorg-to-do-list-agenda/id1238649962) - TO-DO list and agenda app with WebDAV sync support.
- [GoodReader](https://apps.apple.com/app/goodreader-pdf-editor-viewer/id777310222) - PDF viewer and editor that supports WebDAV sync.
- [Joplin](https://apps.apple.com/app/joplin/id1315599797) - Note taking and to-do application that supports WebDAV sync.
- [Notability](https://apps.apple.com/app/notability/id360593530) - Note-taking app that supports webDAV for backups.
- [Notebooks 10](https://apps.apple.com/app/notebooks-write-and-organize/id1490084838) - Writing app, a text and markdown editor with WebDAV support.
- [PotPlayer](https://potplayer.daum.net/) - Windows only.
- [Strongbox](https://apps.apple.com/app/strongbox-password-safe/id897283731) - KeePass-based password manager that supports WebDAV sync.
- [Table Habit](https://github.com/FriesI23/mhabit) – Micro habits tracking app with [sync via WebDAV](https://github.com/FriesI23/mhabit/wiki/Feature%EA%9E%89-WebDAV-Sync). `AL2` `Dart`  `Apache-2.0`


## Libraries

_Libraries for accessing a WebDAV storage and/or building a WebDAV server_

### C

- [neon](https://github.com/notroj/neon) - An HTTP/1.1 and WebDAV client library with a C API.

### C++

- [webdav-client-cpp](https://github.com/CloudPolis/webdav-client-cpp) - C++ WebDAV Client.

### Objective-C / iOS

- https://github.com/mattrajca/DAVKit
- https://github.com/zwaldowski/DZWebDAVClient

### .Net

- https://github.com/saguiitay/WebDAVClient

### Go

- [golang.org/x/net/webdav](https://godoc.org/golang.org/x/net/webdav) - WebDAV server implementation as part of the standard library.
- [go-webdav](https://github.com/emersion/go-webdav) - Client library for WebDAV, CalDAV and CardDAV.
- [gowebdav](https://github.com/studio-b12/gowebdav) - WebDAV client library and command line tool.

### Java

- [Jackrabbit WebDAV Library](https://jackrabbit.apache.org/jcr/components/jackrabbit-webdav-library.html) - WebDAV Library component of the Apache Jackrabbit project. `Apache-2.0`
- [milton2](https://github.com/miltonio/milton2) - Milton Java WebDAV / CalDAV / CardDAV Server Library. `Apache-2.0`
- [sardine](https://github.com/lookfirst/sardine) - Java client based on Apache HTTP Client. `Apache-2.0`
- [sardine-android](https://github.com/thegrizzlylabs/sardine-android) - a WebDAV client for Android based on OkHttp. `Apache-2.0`
- [owncloud/android-library](https://github.com/owncloud/android-library) - an ownCloud library that internally use WebDAV over OkHttp. `MIT`
- [dav4jvm](https://github.com/bitfireAT/dav4jvm) - dav4jvm is a WebDAV/CalDAV/CardDAV library for JVM (Java/Kotlin) developed for DAVx⁵. `MPL-2.0`


### JavaScript and Dart

- [perry-mitchell/webdav-client](https://github.com/perry-mitchell/webdav-client) - WebDAV client written in JavaScript for Node.js and the browser.
- [unifile](https://github.com/silexlabs/unifile) - Node.js library to access cloud storage which supports WebDAV.
- [mikedeboer/jsDAV](https://github.com/mikedeboer/jsDAV) - a Node.js port of SabreDAV with support of many features.
- [nephele](https://www.npmjs.com/package/nephele) - WebDAV, CardDAV, and CalDAV server for Node.js and Express. `Apache-2.0`
- [FriesI23/simple_webdav_client](https://github.com/FriesI23/simple_webdav_client) - Dart library `Dart` `MIT`

### Python

- [webdavclient3](https://pypi.org/project/webdavclient3/) - WebDAV client for Python 3.x.
- [YaDiskClient](https://github.com/TyVik/YaDiskClient) - a simple to use client for Yandex Disk. `MIT`

## Cloud providers

_Cloud services that offer a WebDAV server or otherwise allow access via WebDAV_

- [1und1.de](https://www.1und1.de/) - a hosting and cloud (HiDrive). Based in Germany.
- [4shared](https://www.4shared.com/web/helpCenter/fGeDNHCrXce#par_eight) - Fully supports WebDAV and allows synchronization over it. Based in Ukraine.
- [~Box~](https://support.box.com/hc/en-us/articles/360043696414-WebDAV-with-Box) - Has a WebDAV URL that allows access via WebDAV (no longer supported).
- [CloudMe](https://www.cloudme.com/en/webdav) - cloud solution.  Based in Sweden.
- [EDIS](https://www.edis.at/) - a (web) server and infrastructure hoster. Based in Austria.
- [FastMail](https://www.fastmail.help/hc/en-us/articles/1500000277882-Remote-file-access) - an Email service with WebDAV access to files. Based in Australia.
- [GM Cloud](https://www.gmx.com/cloud/) -  a Web portal with cloud feature. Based in Germany.
- [IceDrive](https://icedrive.net/) - a cloud solution. Based in UK.
- [infomaniak](https://www.infomaniak.com/) - The Ethical Cloud and colaboration service. Based in Switzerland.
- [IONOS](https://www.ionos.com/) - a hosting and cloud (HiDrive). Based in US.
- [Jianguoyun / Nutstore](https://www.jianguoyun.com/) - a cloud and workspace. Based in China.
- [Kolab Now](https://kb.kolabnow.com/faq/can-i-access-my-files-via-webdav) - a collaboration service. Based in Switzerland.
- [Koofr](https://koofr.eu/) - a personal cloud services. Based in Slovenia.
- [luckycloud](https://docs.luckycloud.de/en/cloud-storage/webdav) - an advanced cloud. Based in Germany.
- [mail.com](https://www.mail.com/) - an Email service but also provides WebDAV access to stored files.
- [MyDrive](https://www.mydrive.ch/) - s cloud solution. Based in Switzerland.
- [OpenDrive](https://www.opendrive.com/) - a cloud and office suite. Based in US.
- [pCloud](https://www.pcloud.com/) - business level accounts can use WebDAV.
- [STRATO](https://www.strato.com/) - a hosting and cloud (HiDrive). Based in Germany, Netherlands, Spain, France, UK, Sweden.
- [T-Online.de / Magenta](https://cloud.telekom-dienste.de/) - a ISP and cloud. Based in Germany.
- [transip.nl](https://www.transip.nl/) - an ISP that offers cloud. Based in the Netherlands.
- [web.de](https://hilfe.web.de/cloud/netzlaufwerk/windows-10.html) - a Web portal with cloud feature. Based in Germany.
- [Woelkli](https://woelkli.com/) - a NextCloud-based service. Based in Switzerland.
- [Yandex.Disk](https://yandex.com/dev/disk/webdav/) - Has a WebDAV API that treats its storage like a file system. Based in Russia.
- [Zaclys](https://www.zaclys.com/) - a NextCloud-based service. Based in France.

Comparision of the providers:
  * [Linux и бесплатные облачные хранилища, семь лет спустя](https://habr.com/ru/articles/651609/)

## Extensions

_Protocol extensions and related protocols_

- [CalDAV](https://en.wikipedia.org/wiki/CalDAV)
- [CardDAV](https://en.wikipedia.org/wiki/CardDAV)
- [Microsoft Extensions](https://docs.microsoft.com/en-us/openspecs/sharepoint_protocols/ms-wdvme/8cafdf55-ee5c-443e-bdb7-2cb2ab1fb2c3)

## Contributing

Contributions welcome! Read the [contribution guidelines](contributing.md) first.
