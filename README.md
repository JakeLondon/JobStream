jobstream
===================================


Requires£º

X86 CPU
Linux Kernel Version >= 2.6.18
Host OR VM (KVM,XEN,Vmware, etc)
Installation

$git clone https://github.com/zzgang/kconnp.git
$cd kconnp
$./configure
$make
$make install
Usage

Commands

kconnp (stats|ldcfg|start|stop|restart)

stats: output the statistics infomation
ldcfg: reload the config
start: start the service
stop: shutdown the service
restart: restart the service
Configuration

Files

Global: /etc/kconnp.conf
White list for ACL: /etc/iports.allow
Black list for ACL: /etc/iports.deny
Explains

The priority of black list is higer than white black list.
If the iport is specified£¬the connections will be precommectted.
If the connection is configured stateful (tag: (S))£¬each connection only be use one time before closing.
E-Mail:£ºzzgang2008@foxmail.com
