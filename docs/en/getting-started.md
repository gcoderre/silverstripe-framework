## What is SilverStripe?

SilverStripe is a content management system built on top of a PHP programming framework. It is used to build websites, intranets and web applications.

Besides a powerful and intuitive content authoring application, SilverStripe contains a powerful PHP5-based programming framework. The SilverStripe Framework brings immense flexibility and ease in customising your site and provides fundamentals such as security models, workflow, caching, and multiple language and subsite support.

SilverStripe CMS is open source, underpinned by public documentation, free code, and a developer community. It is based on open standards and supports multiple technology platforms. 

## Requirements

SilverStripe needs to be installed on a web server. Content authors and website administrators use their web browser to access a web-based GUI to do their day-to-day work. Website designers and developers require access to the files on the server to update templates, website logic, and perform upgrades or maintainance.

### Required libraries

* PHP 5.3.2+ with at least 48mb of memory allocated to each PHP process
* The following PHP modules: dom, gd2, fileinfo, hash, iconv, mbstring, mysql (or other database driver), session, simplexml, tokenizer, xml.

### Compatible operating systems

* Linux / UNIX / BSD
* Microsoft Windows XP SP3, Vista, Windows 7, Server 2008, Server 2008 R2
* Mac OS X 10.4+

### Compatible web servers

* Apache 2.0+ with mod_rewrite and "AllowOverride All" set
* IIS 7+
* Nginx
* Lighttpd

### Compatible database systems

* MySQL 5.0+ (default)
* PostgreSQL 8.3+ (requires [postgresql](http://silverstripe.org/postgresql-module) module)
* SQL Server 2008+ (requires [mssql](http://silverstripe.org/microsoft-sql-server-database/) module)

Support for [Oracle](http://www.silverstripe.org/oracle-database-module/) and [SQLite](http://silverstripe.org/sqlite-database/) is not commercially supported, but is under development by our open source community.

## Installation

The prefered way to install SilverStripe is with the [Composer](http://getcomposer.org/doc/00-intro.md) package manager.

```
# Make sure you're using the latest version of Composer
~ sudo composer self-update
```

```
# Create a project using the latest stable version of SilverStripe
composer create-project silverstripe/installer ./my/website/folder
```

The public directory of SilverStripe is its root directory. In this case, `./my/website/folder`.

You can create a project using a specific version of SilverStripe by specifying a release version like below.

```
composer create-project silverstripe/installer ./my/website/folder 3.0.3
```

### Other tasks available through Composer

Adding modules to your project

```
composer require silverstripe/forum:*
```

Searching for silverstripe modules

```
composer search silverstripe
```

Updating dependencies

```
composer update --no-dev
```

To use development versions of SilverStripe, see the [Contributing code](/contributing/code) page.

### Installing from source

If you do not wish to install SilverStripe with Composer, you can [download SilverStripe](http://silverstripe.org/download) from the website.
