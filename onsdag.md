Wednesday
===

# Keynotes

* oci/cri  er ipv6 native !!!

* Prometheus 2.0
	* better than 1.0...

* https://linkerd.io/
	* couple with conduit to get pretty things

* [kata containers](https://katacontainers.io)
	* toughening of containers

* [envoy](https://github.com/envoyproxy/envoy)
	* C++ (ugh) edge-proxy for services
	* [source](https://github.com/envoyproxy/envoy)

* [TUF](https://theupdateframework.github.io)
	* Update Framework
	* [source](https://github.com/theupdateframework/tuf)

[CNCF landscape](https://github.com/cncf/landscape)

![landscape](https://github.com/cncf/landscape/raw/master/landscape/CloudNativeLandscape_latest.jpg)

## jaeger
opentracing from uber

donated to CNCF, looks nice

## Fluentd

* now exports prometheus metrics
* v1.0 is out, put it in k8s
* [700 plugins]( https://www.fluentd.org/plugins)


## conduit
[why have a service mesh](https://buoyant.io/2017/04/25/whats-a-service-mesh-and-why-do-i-need-one/)

looks nice, how much control is lost?

```
# monitor live intra-service traffic
conduit tap

# visualise intra-service networking
conduit dashboard
```

## spinnaker

*netfix CI / infrastructure management*

* pluggable arch

* does "everything" and blurs (pollutes?) the lines between ci and cd, testing and resilience testing

* supports regional deployments to perform green/blue at regional level

* support for "manual judgement" push button (*noice*)

*lots of yada-yada about culture*

## AWS Cloud native principles
*Adrian Cockroft*

* [fargate](https://aws.amazon.com/blogs/aws/aws-fargate/)
	* Run Containers without Managing
	* Runs on EKS [elastic kubernetes service](https://aws.amazon.com/eks/)
* [re:invent talk ARC219 youtube](https://www.youtube.com/watch?v=aLSFGLJ6Byo)
* [Adrian Cockroft on Medium](medium.com/@adrianco)
* Native VPC networking with CNI plugin on AWS
	* [open source on github](https://github.com/aws/amazon-vpc-cni-k8s)
* [SPIFFE](https://spiffe.io)
	* seems not ready, more of an initiative?
	* aims to replace things like vault?

## ISTIO

* sidecar based arch
* control plane
^ intercepts all traffic
* adds telemetry
* adds tracing
* no code change demands

* based on envoy
	* not necessary to use envoy


Good points
* consistent metrics across fleet, no instrumenting needed in-app
* tracing --"--
