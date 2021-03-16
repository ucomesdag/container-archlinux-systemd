Archlinux Systemd Container Image
========================

This Containerfile can build containers capable to use systemd.

[![archlinux build status](https://quay.io/repository/ucomesdag/archlinux/status "Container Repository on Quay")](https://quay.io/repository/ucomesdag/archlinux)

Branches
--------

This repository has multiple branches that relate to Archlinux versions.

|Branch |Archlinux Version|Container image tag|
|-------|-----------------|-------------------|
|main   |latest           |latest             |

Pull strategy
-------------

The different branches are **not** merged, they live as individual branches.

Manually starting
-----------------

```
podman run \
  --tty \
  --privileged \
  --volume /sys/fs/cgroup:/sys/fs/cgroup:ro \
  quay.io/ucomesdag/archlinux
```
