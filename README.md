Harvester Load Balancer
==========================
[![Build Status](https://drone-publish.rancher.io/api/badges/harvester/load-balancer-harvester/status.svg)](https://drone-publish.rancher.io/harvester/load-balancer-harvester)
[![Go Report Card](https://goreportcard.com/badge/github.com/harvester/load-balancer-harvester)](https://goreportcard.com/report/github.com/harvester/load-balancer-harvester)
[![Releases](https://img.shields.io/github/release/harvester/load-balancer-harvester/all.svg)](https://github.com/harvester/load-balancer-harvester/releases)

Harvester Load Balancer is a load balancing controller. Combined with other components like [kube-vip](https://github.com/kube-vip/kube-vip) and [Harvester CCM](https://github.com/harvester/cloud-provider-harvester), it makes Harvester a cloud provider.
Users can deploy Harvester Load Balancer in any other Kubernetes clusters without dependency on Harvester.

## Deploying
```
# helm v3
helm install harvester-load-balancer deploy/harvester-load-balancer -n harvester-system --set kube-vip.interface=<interface name> --set kube-vip.address=<IP address>
```

## License
Copyright (c) 2020 Rancher Labs, Inc.

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.

