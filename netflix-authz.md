# Netflix authorization talk (OPA ftw)
* Details [on sched.com](https://kccncna17.sched.com/event/CU73/how-netflix-is-solving-authorization-across-their-cloud-i-manish-mehta-torin-sandall-netflix)
* Slides [on schd.ws](https://schd.ws/hosted_files/kccncna17/cb/Manish%20Mehta%20Netflix%20AuthZ%20V4.pdf)
* Youtube-video coming up

### Problem presented:
* Authorization is hard, and slow.
* Network latency is a bottleneck when creating authorization-based services
* Usually, you trade performance for some semblance of security

### Product pushed as solution: [Open Policy Agent (opa)](https://github.com/open-policy-agent/opa)
* Designed with performance as the primary goal
* 98.8% Golang
* In-memory cache
* Library / host-local agent
* Can be run as sidecar or library
* Easy to use (or so they say)
* Uses a custom declarative policy language, called Rego
  * Built around the assumption of a REST/graph API
  * Supports permission groups and group hierarchies
  * Namespaced for concise permission naming

### QA notes
* istio may solve some of the same problems