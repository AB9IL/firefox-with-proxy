# Firefox-with-proxy

A wrapper for running Firefox with Proxychains, providing sophisticated proxying for Tor or other anti-censorship or anonymity tools. This script watches a flag set by other software and toggles firefox between proxified and in-the-clear operation.

## Requires:

Firefox browser and Proxychains.
Works with the anti-censorship / pro-anonymity tools in [MOFO Linux](https://mofolinux.com/index.html), [Catbird Linux](https://catbirdlinux.com/index.html), or [Skywave Linux](https://skywavelinux.com/index.html) as installed.

## Desccription:

This is a wrapper for Firefox which switches to proxified browsing if other software creates a file "/tmp/proxyflag" or non-proxified without it. In Ubuntu or Debian Linux, use _update-alternatives_ to set x-www-browser path to this script (e.g. /usr/local/sbin/firefox-with-proxy). Tor-controller, tor-remote, or other proxying scrpts should set or remove the proxyflag as needed. If all works correctly, you may open Firefox and experience smooth, seamless operation in either configuration. 
