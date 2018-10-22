# ![Icon](./.bluemix/secure-lock-kubernetes.png) Exposing Service in SDT with ISTIO


### Register an access endpoint to ISTIO for service running in WH SDT Kubernetes Cluster
This is a DevOps toolchain that is preconfigured for register service access endpoint with ISTIO service running in SDT K8S cluster, to expose a endpoint in BlueZone for dev/test purpose.

Istio routing rules is pre-defined in source control, along with its Kubernetes deployment script.
The target service is configured with ISTIO during toolchain setup (using a Bluemix API key, cluster name, service name and namespace of cluster). You can later change these by altering the Delivery Pipeline configuration.
Any code change to the routing rules repo will automatically be built, validated and update the routing policy in the Kubernetes cluster for the target service.

![Icon](./.bluemix/toolchain.png)

### To get started, click this button:
[![Deploy To Bluemix](https://console.bluemix.net/devops/graphics/create_toolchain_button.png)](https://console.bluemix.net/devops/setup/deploy/?repository=https%3A//github.com/yeungbo/secure-kube-toolchain)


---
### Toolchain Configuration Help
#### (1) _Toolchain_
**Toolchain Name:** `Toolchain name` (Update toolchain name as needed)<br/>
**Select Region:** `IBM Cloud region`<br/>
**Select a resource group:** `IBM Cloud resource group`<br/>
#### (2) _Git Repos_
**Repository type:** `clone`<br/>
**Source repository URL:** `https://github.com/yeungbo/register-service-with-istio`<br/>
**Owner:** `Git owner or group name`<br/>
**Repository Name:** `New git project/repo name` (Update repo name as needed)<br/>
#### (3) _Delivery Pipeline_
**App name:** `Name for the toolchain instance`<br/>
**Service name:** `Service name in k8s cluster`<br/>
**Cluster Namespace name:** `IBM Kubernates cluster deployment namespace that service running in`<br/>
**Access Endpoint name:** `Access Endpoint name to register on ISTIO`<br/>
**IBM Cloud API Key:** `IAM key to IBM Kubernates cluster` (create ahead)<br/>
**Region:** `The IBM Cloud region`<br/>
**Cluster Name:** `IBM Kubernates cluster name`<br/>
#### (4) _Slack_
**Slack webhook:** `Slack webhook URL`<br/>
**Slack channel:** `#Slack channel Name`<br/>
**Slack team name:** `ibm-watsonhealth`<br/>


---
### Learn more 

* User Guide [Exposing YOUR Service with ISTIO service](https://apps.na.collabserv.com/wikis/home?lang=en-us#!/wiki/Wa0a1d43ca7a0_4fff_87ff_04006c762969/page/Exposing%20YOUR%20Service%20with%20ISTIO%20service)
* [Documentation](https://apps.na.collabserv.com/wikis/home?lang=en-us#!/wiki/Wa0a1d43ca7a0_4fff_87ff_04006c762969/page/Multi-tenant%20Exposing%20Service%20with%20ISTIO)
