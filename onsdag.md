Onsdag
===

* oci/cri  er ipv6 native !!!

* Prometheus 2.0

* https://linkerd.io/

* [kata containers](https://katacontainers.io)

* [envoy](https://github.com/envoyproxy/envoy)
	* C++ (ugh)
	* [source](https://github.com/envoyproxy/envoy)

* [TUF](https://theupdateframework.github.io)
	* Update Framework
	* [source](https://github.com/theupdateframework/tuf)

[CNCF landscape](https://github.com/cncf/landscape)

![landscape](https://github.com/cncf/landscape/raw/master/landscape/CloudNativeLandscape_latest.jpg)

## jaeger
opentracing fra uber

## Fluentd

* koble på prometheus
* se på v1.0
* [700 plugins]( https://www.fluentd.org/plugins)


## conduit
[why have a service mesh](https://buoyant.io/2017/04/25/whats-a-service-mesh-and-why-do-i-need-one/)

```
conduit tap

conduit dashboard
```

## spinnaker

*netfix CI / infrastructure management*

* pluggable arch

* gjør "alt" og forurenser linjene mellom ci og cd, testing og resilience testing

* støtter regionale deployments for å gjøre green/blue på region-nivå

* support for "manual judgement" push button (*noice*)

## AWS Cloud native principles

* [fargate](https://aws.amazon.com/blogs/aws/aws-fargate/)
	* Run Containers without Managing Infrastructure
	* 
* re:invent tal ARC219 youtube
* medium.com/@adrianco
* Native VPC networking with CNI plugin on AWS
	* open source on github
* 