# DevOps Engineer - technical interview
## Testing goals
  * With this test, we want to see your ability to create an entire infrastructure from scratch as well as your skills as a system administrator.
## The task
  * Your task is to provision a highly available Kubernetes Environment along with a webserver that has MySQL as backend and nginx/httpd as frontend proxy. The cluster should not be publicly available, while the webserver should be accessible via port 443.
## The solution
  * In your solution please emphasize on readability, maintainability and DevOps methodologies. We expect a clear way to recreate your setup.
  * The webserver must have a valid certificate.
  * Use Ansible as the configuration management for server setup, webserver config and use RKE for Kubernetes cluster creation. 
  * Kubernetes nodes should be placed on VM's instead of the main servers. 
  * Inter node connections must be handled via VPN, preferably WireGuard.
  * The infrastructure provider can be AWS/DO/GCP.
  * Servers and Nodes should run on Ubuntu 20.04, using security best practices.
  * Should leverage community roles when it make sense.
  * Generic RBAC setup for Kubernetes.
  * A clean bare minimum working infrastructure is preferred than a full blown solution pieced together with scissors, rope and duct tape. Do not skip security considerations.
## When you are finished
  * Submit your solution to a Github repository and send us a link.
  * Make sure your README tells us how to run it.
  * Please fork this repo so that you are tested against the test that you started with as this test may change.
## Bonus Points
  * If you use ansible vault / HashiCorp Vault for encrypting sensitive information.
  * If you can document all aspects of your code, in the README and within the code itself.
  * If you can generate the self signed cert/key.
  * If you can make this run all in one playbook.