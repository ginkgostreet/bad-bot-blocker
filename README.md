Bad Bot Blocker
===============

Apache htaccess rules to block bad bots.

Bad bots are defined as:

- E-mail harvesters
- Content scrapers
- Spam bots
- Vulnerability scanners
- Aggressive bots that provide little value
- Bots linked to viruses or malware
- Government surveillance bots
- Russian search engine Yandex
- Chinese search engine Baidu

Yandex/Baidu
------------

Unless your website is written in Russian or Chinese, you probably don't
get any traffic from them. They mostly just waste bandwidth and consume resources.


Bots Are Liars
--------------

Bots try to make themselves look like other software by disguising their
useragent. Their useragents may look harmless, perfectly legitimate even.
For example, "^Java" but according to
[Project Honeypot](https://www.projecthoneypot.org/harvester_useragents.php),
it's actually one of the most dangerous.


Setup
-----

This should be added to the site .htaccess file just after the php version
is set and defaults file on Siteground sites. Best discretion on where this
goes is advised. Assumes you have other rewrite rules in place.

If you have a bizarre or complicated setup, be sure to look everything
over before using it. But for anyone with something that resembles
a standard Apache installation, this should work without any issues.
