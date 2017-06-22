---
ID: 3105
post_title: deutschland iptables
author: rogera
post_date: 2017-06-22 09:00:39
post_excerpt: ""
layout: post
permalink: >
  http://wolfspool.at/wprcs1/deutschland-iptables/
published: true
fusion_builder_status:
  - ""
---
root@deutschland ~ # iptables -t nat -A POSTROUTING -o eth0 -j MASQUERADE
root@deutschland ~ # iptables -A FORWARD -i eth0 -o eth0:1 -m state --state RELATED,ESTABLISHED -j ACCEPT
root@deutschland ~ # iptables -A FORWARD -i eth0:1 -o eth0 -j ACCEPT
root@deutschland ~ # iptables --list -v

nach: http://www.yourownlinux.com/2013/07/how-to-configure-ubuntu-as-router.html