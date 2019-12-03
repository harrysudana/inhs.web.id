---
title: "Remote Fatal Unable to Create Thread Resource Temporarily Unavailable"
date: 2019-10-26T02:41:52+08:00
draft: false
Tags: ["CPanel"]
---

![Permasalahan](/img/remote-fatal-unable-to-create-thread-Resource-temporarily-unavailable.png)

Permasalahan pada saat git pull dari repository client yang menggunakan shared hosting CPanel dengan status remote: fatal: unable to create thread: Resource temporarily unavailable

Hasil pencarian didapatkan hasil dari [stackoverflow](https://stackoverflow.com/questions/9905257/git-push-fatal-unable-to-create-thread-resource-temporarily-unavailable) dengan menaikkan pack.threads di shared hosting milik client.

`git config --global pack.threads "5"`


![Hasil](/img/solusi-git-config.png)

Referensi :
https://stackoverflow.com/questions/9905257/git-push-fatal-unable-to-create-thread-resource-temporarily-unavailable