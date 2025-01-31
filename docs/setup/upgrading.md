---
title: Upgrading your Snikket instance
linktitle: Upgrading
description: "Upgrading your Snikket instance is easy."
date: 2021-05-19T14:32:02Z
weight: 20
---

We periodically announce new releases of the Snikket server software on our
[blog][], [Mastodon][] and [Twitter][]. You will also receive [update
notifications][] directly from your instance when it is time to upgrade.

Upgrading to a new Snikket release is typically very easy. The correct process
to use depends on the method you initially used to set up your Snikket
instance. Each method is explained here.


{{< panel style="warning" >}}
**Important note for ARM or Raspberry Pi users:** Some compatibility issues
have been observed with the new release on systems running Debian or Raspbian
10 ("buster") or older. For further advice on this issue, see our
[troubleshooting guide](../troubleshooting/#problems-on-debianraspbian-10-buster-on-raspberry-pi-or-arm-devices).
{{< /panel >}}

## Snikket quick-start

If you are using a version installed from the [original quick-start][] guide
on the website, use these commands:

```
    cd /etc/snikket
    docker-compose pull
    docker-compose up -d
```

## snikket-selfhosted

If you installed Snikket using the [snikket-selfhosted][] scripts, simply run:

```
    cd /opt/snikket
    git pull
    ./scripts/update.sh
```

## Snikket hosting

If you're using our hosting service, you can upgrade by visiting your
[hosting dashboard][] and clicking the 'Update' button next to your instance.

**Note:** Updates are not always available on the hosted platform immediately
after release. If the 'Update' button is not present, try again later.
Typically you will receive a notification when an update is available.

[snikket-selfhosted]: https://github.com/snikket-im/snikket-selfhosted
[original quick-start]: https://snikket.org/service/quickstart/
[hosting dashboard]: https://my.snikket.org/
[blog]: https://snikket.org/blog/
[Mastodon]: https://fosstodon.org/@snikket_im
[Twitter]: https://twitter.com/snikket_im
[update notifications]: ../../advanced/update_notifications/
