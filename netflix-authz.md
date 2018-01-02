# How Netflix Is Solving Authorization Across Their Cloud
<details>
	<summary>Talk details</summary>
	<ul>
		<li>Speakers: Manish Mehta & Torin Sandall</li>
		<li><a href="https://youtu.be/R6tUNpRpdnY">Youtube-video</a></li>
		<li><a href="http://sched.co/CU73">Talk details on sched.com</a></li>
		<li><a href="https://schd.ws/hosted_files/kccncna17/cb/Manish%20Mehta%20Netflix%20AuthZ%20V4.pdf">Slides on schd.ws</a></li>
	</ul>
</details>

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