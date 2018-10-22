# ![Icon](./.bluemix/secure-lock-kubernetes.png) Develop a Kubernetes app


### Register a service access endpoint to ISTIO for service running in WH SDT Kubernetes Cluster
This is a DevOps toolchain that is preconfigured for register service access endpoint with ISTIO service running in SDT K8S cluster, to expose a endpoint in BlueZone for dev/test purpose.

Istio routing rules is pre-defined in source control, along with its Kubernetes deployment script.
The target service is configured with ISTIO during toolchain setup (using a Bluemix API key, cluster name, service name and namespace of cluster). You can later change these by altering the Delivery Pipeline configuration.
Any code change to the routing rules repo will automatically be built, validated and update the routing policy in the Kubernetes cluster for the target service.

![Icon](./.bluemix/toolchain.png)

### To get started, click this button:
[![Deploy To Bluemix](https://console.bluemix.net/devops/graphics/create_toolchain_button.png)](https://console.bluemix.net/devops/setup/deploy/?repository=https%3A//github.com/yeungbo/secure-kube-toolchain)

---
### Learn more 

* User Guide [Exposing YOUR Service with ISTIO service](https://apps.na.collabserv.com/wikis/home?lang=en-us#!/wiki/Wa0a1d43ca7a0_4fff_87ff_04006c762969/page/Exposing%20YOUR%20Service%20with%20ISTIO%20service)
* [Documentation](https://apps.na.collabserv.com/wikis/home?lang=en-us#!/wiki/Wa0a1d43ca7a0_4fff_87ff_04006c762969/page/Multi-tenant%20Exposing%20Service%20with%20ISTIO)
