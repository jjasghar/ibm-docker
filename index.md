---
layout: default
---

---

## You're here because...

* You want to use [docker][docker] as your environment to talk to the IBM Cloud.
* You don't want to use the `install.sh` or `curl || bash` something to your machine.

## Prerequisite

You will need docker installed on your machine, or a place you can used the `docker pull` commands.

## Containers

These will be from the smallest to the largest pulls. Please pay attention to the class you are
in if you don't know which to use. Otherwise, each of these should fit your use case when using
the IBM Cloud.

### ibm-cloud-cli

This container is everything you need for the [Kube101][kube101] class. It is as stripped down
as possible and only gives you the minimal of what you need.

```shell
docker pull jjasghar/ibm-cloud-cli
```

Based off of Alpine, it has the following to interface with the IBM Cloud. If you have any suggestions
or thoughts, don't hesitate to PR [here](https://github.com/jjasghar/ibm-cloud-cli).

- `ibmcloud`
  - `container-service`
  - `container-registry`
- `kubectl`

### ibm-cloudnative-tools

This container is everything you need for the [Kube101][kube101] and [Istio101][istio101] class.

```shell
docker pull jjasghar/ibm-cloudnative-tools
```

It is based off of Debian, and the following to interface with the IBM Cloud. If you have any suggestions
or thoughts, don't hesitate to PR [here](https://github.com/jjasghar/ibm-cloudnative-cli).

- `git`
- `helm`
- `ibmcloud`
- `istioctl`
- `kubectl`
- `nano`

### ibm-cloud-tools

This is the container with every integration I could find to talk to the IBM Cloud.

```shell
docker pull jjasghar/ibm-cloud-tools
```

It is based off of Debian, and the following are all included in this container. If you have any suggestions
or thoughts, don't hesitate to PR [here](https://github.com/jjasghar/ibm-cloud-tools).

- `git`
- `helm`
- `ibmcloud`
- `istioctl`
- `kubectl`
- `nano`
- `slcli`
- `terraform`

### License & Authors

- Author: JJ Asghar <jja@ibm.com>

```text
Copyright:: 2018- IBM, Inc

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```

[docker]: https://www.docker.com/
[kube101]: https://github.com/IBM/kube101
[istio101]: https://github.com/IBM/istio101
