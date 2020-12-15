# ClickHouse Docker Image for Podman/OpenShift/OKD

[![ClickHouse][ClickHouse-badge]][clickhouse-url]
[![OpenShift][OpenShift-badge]][openshift-url]
[![License][license-badge]][license-url]
[![Build Status][build-badge]][build-url]

A stripped version of the [original ClickHouse Docker image][clickhouse-docker].

The primary difference is that `USER`, `gosu`, `chmod` and hard-coded users
have been removed. This image is compatible with Podman/OpenShift/OKD and
doesn't require root permissions to run.

```bash
podman pull quay.io/kryptonite/clickhouse-docker-rootless:20.9.3.45
```

## See Also

- [ClickHouse][clickhouse]
- [ClickHouse Docker Image][clickhouse-docker]
- [ClickHouse Operator][clickhouse-operator]
- [Podman][podman]

[build-badge]: https://quay.io/repository/kryptonite/clickhouse-docker-rootless/status
[build-url]: https://quay.io/repository/kryptonite/clickhouse-docker-rootless
[license-badge]: https://img.shields.io/badge/License-Apache--2.0-blue.svg?style=flat
[license-url]: LICENSE
[clickhouse-badge]: https://img.shields.io/badge/ClickHouse-DBMS-yellow.svg?style=flat
[clickhouse-url]: https://github.com/ClickHouse/ClickHouse
[openshift-badge]: https://img.shields.io/badge/OpenShift-4.x-orange.svg?style=flat
[openshift-url]: https://docs.openshift.com/container-platform/4.5/openshift_images/create-images.html#images-create-guide-general_create-images

[clickhouse]: https://github.com/ClickHouse/ClickHouse
[clickhouse-docker]: https://github.com/ClickHouse/ClickHouse/tree/master/docker/server
[clickhouse-operator]: https://github.com/Altinity/clickhouse-operator
[podman]: https://podman.io/
