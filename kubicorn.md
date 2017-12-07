# Building a cluster management API using kubicorn
<details>
	<summary>Talk details</summary>
	<ul>
		<li>Speakers: <a href="https://twitter.com/kris__nova">Kris Nova</a> (Heptio) & <a href="https://github.com/roberthbailey">Robert Bailey</a> (Google)</li>
		<li>Youtube-video: Coming up</li>
		<li><a href="http://sched.co/CU67">Talk details on sched.com</a></li>
	</ul>
</details>

### Problems
* Setting up a K8S instance is hard
* Migrating between cloud providers is hard

### Solution
* Tool: [kubicorn](https://github.com/kris-nova/kubicorn)
* 88.9% Go
* Lets you create a declarative representation of a cluster and apply it consistently across multiple cloud environments
* yaml-based
  * provider-specific configs are isolated into blocks
* Uses kubectl
  * `kubectl get machines`
  * `kubectl get nodes`
  * `kubectl create -f machine.yaml`
* Many node- and cluster-related utilities, i.e.:
  * Tool to upgrade nodes in cluster: `./upgrader -v 1.8.3`
  * Live demo during talk, youtube video recommended


#### Other tools to possibly look at:
* Kops
* AKS
* Stackpoint
* Kraken
* Bootkube
* Kubo
* Kubespray
* Kismatic