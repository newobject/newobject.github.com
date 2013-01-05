---
layout: post
title: "Multiple ssh keys"
description: ""
category: tips
tags: [ssh]
---
{% include JB/setup %}

Edit the ~/.ssh/config:

    Host github github.com
    Hostname github.com
    IdentityFile ~/.ssh/newobject_rsa

    Host bitbucket bitbucket.org
    Hostname bitbucket.org
    IdentityFile ~/.ssh/newobject_rsa

    Host kabam 10.80.0.201
    Hostname 10.80.0.201
    IdentityFile ~/.ssh/kabam_rsa


[http://stackoverflow.com/questions/2419566/best-way-to-use-multiple-ssh-private-keys-on-one-client](http://stackoverflow.com/questions/2419566/best-way-to-use-multiple-ssh-private-keys-on-one-client)
