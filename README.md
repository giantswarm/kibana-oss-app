[![CircleCI](https://circleci.com/gh/giantswarm/kibana-oss-app.svg?style=shield)](https://circleci.com/gh/giantswarm/kibana-oss-app)

# kibana-oss-app chart

Giant Swarm offers a kibana-oss Managed App which can be installed in tenant clusters.
Here we define the kibana-oss chart with its templates and default configuration.

This is the official Kibana - OSS from Elastic adjusted to run on GS clusters.

## Configuration
By default Kibana will be configured for Elastic Search at `http://elasticsearch-master:9200`
Please provide valid `elasticsearchHosts` address for your custom setup.

More configuration will come in the future

## Installation
After providing valid `elasticsearchHosts` or `elasticsearchURL` for your setup, you can install it via:

helm install -n kibana giantswarm-playground-catalog/kibana-oss-app

## Compatibility
Tested on Giant Swarm release 11.2.0 on Azure with Kubernetes 1.16.3

## Credit

* https://github.com/elastic/helm-charts/tree/master/kibana
