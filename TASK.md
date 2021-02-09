# DevOps Engineer - technical interview
## Testing goals
  * With this test, we want to see your ability to create an entire infrastructure from scratch as well as your skills as a system administrator.
## The task
  * Your task is to provision a highly available Kubernetes Environment along with a webserver running inside 'aigent-test' namespace, that has MySQL as backend and nginx/httpd/haproxy as frontend proxy. 
  * The cluster should not be publicly available, while the webserver should be accessible via port 443, the proxy can be ran outside of the cluster. 
## The solution
  * In your solution please emphasise on readability, maintainability and DevOps methodologies. We expect a clear way to recreate your setup. 
  * The webserver must have a valid certificate.
  * Use Ansible as the configuration management for server setup and hardening.
  * Webserver can be configured based on preference.
  * Use RKE for Kubernetes cluster creation.
  * Inter node connections must be handled directly via VPN, preferably WireGuard, ssh to the servers must be also handled via VPN.
  * The infrastructure provider can be AWS/DO/GCP etc. 2 machines are enough.
  * Servers must run on Ubuntu 20.04.
  * Should leverage community roles when it make sense.
  * Requirements for Kubernetes: 
   -RBAC, 
   - 2x namespaces : aigent-test, monitoring
  * 'aigent-test' should have the webserver service, and 'monitoring' should just have a simple Grafana service, with server stats pushed into it. 
  * A clean bare minimum working infrastructure is preferred than a full blown solution pieced together with scissors, rope and duct tape. Do not skip security considerations.
## When you are finished
  * Submit your solution to a GitLab repository and send us a link.
  * Provide us a Wireguard config and k8s config to access the cluster and underlying servers.
  * Make sure your README mentions important details about your project, like IPs, cluster name, etc. 
  * Please fork this repo so that you are tested against the test that you started with as this test may change.
## Bonus Points
  * If you use ansible vault / HashiCorp Vault for encrypting sensitive information.
  * If you can document all aspects of your code, in the README and within the code itself.
  * If you can generate the self signed cert/key.
  * If you can make most of this run in an Ansible Playbook. 
