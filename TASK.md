# DevOps Engineer - technical interview
## Testing goals
  * With this test, we want to see your ability to create an entire infrastructure from scratch as well as your skills as a system administrator.
## The task
  * Your task is to create a *TEMPLATE* for a highly available Kubernetes Environment with a webserver that has MySQL as backend and nginx/httpd as frontend proxy.
  * We mainly expect configuration files for Kubernetes, and k8s.yamls for the webserver and mysql. Please detail the steps you would take for each item.
## The solution
  * In your solution please emphasize on readability, maintainability and DevOps methodologies. We expect a clear way to recreate your setup.
  * The webserver must have a valid certificate and must be publicly available via port 443.
  * Kubernetes template should be created for RKE. (https://rancher.com/docs/rke/latest/en/)
  * We expect some generic RBAC yamls for Kubernetes.
  * A clean bare minimum working infrastructure is preferred than a full blown solution pieced together with scissors, rope and duct tape. Do not skip security considerations.
## When you are finished
  * Submit your solution to a Github repository and send us a link.
  * Make sure your README tells us how to run it.
  * Please fork this repo so that you are tested against the test that you started with as this test may change.
## Bonus Points
  * If you use ansible vault / HashiCorp Vault for encrypting sensitive information.
  * If you can make Kubernetes accessible only via VPN (preferably WireGuard)
  * If you can document all aspects of your code, in the README and within the code itself.
  * If you can generate the self signed cert/key.
  * If you can use Ansible for any items mentioned.
  * If you can show us a demo of your configuration (locally via Minikube for example.)
