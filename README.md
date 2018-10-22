# ![Icon](./.bluemix/secure-lock-kubernetes.png) Exposing Service in SDT with ISTIO


### Register an access endpoint to ISTIO for service running in WH SDT Kubernetes Cluster
This is a DevOps toolchain that is preconfigured for register service access endpoint with ISTIO service running in SDT K8S cluster, to expose a endpoint in BlueZone for dev/test purpose.

Istio routing rules is pre-defined in source control, along with its Kubernetes deployment script.
The target service is configured with ISTIO during toolchain setup (using a Bluemix API key, cluster name, service name and namespace of cluster). You can later change these by altering the Delivery Pipeline configuration.
Any code change to the routing rules repo will automatically be built, validated and update the routing policy in the Kubernetes cluster for the target service.

![Icon](./.bluemix/toolchain.png)

### To get started, click this button:
[![Deploy To Bluemix](https://console.bluemix.net/devops/graphics/create_toolchain_button.png)](https://console.bluemix.net/devops/setup/deploy/?repository=https%3A//github.com/yeungbo/secure-kube-toolchain)


Toolchain Configuration Help
(1) Toolchain

Toolchain Name: Toolchain name (Update toolchain name as needed)
Select Region: CF region
Choose an organization: CF organization
(2) Git Repos

Repository type: clone
Source repository URL: https://github.ibm.com/whc-toolchain/whc-nodejs-starter
Owner: Git owner or group name
Repository Name: New git project/repo name (Update repo name as needed)
(3) Delivery Pipeline

App name: Service name
IBM Cloud API Key: IAM key to IBM Kubernates cluster (create ahead)
Container registry region: Container registry region
Container registry namespace: Container registry namespace (create ahead)
Cluster region: CF region
Cluster name: IBM Kubernates cluster name
Cluster namespace: IBM Kubernates cluster deployment namespace (create ahead)
(4) Slack

Slack webhook: Slack webhook URL
Slack channel: #Slack channel Name
Slack team name: ibm-watsonhealth

---
### Learn more 

* User Guide [Exposing YOUR Service with ISTIO service](https://apps.na.collabserv.com/wikis/home?lang=en-us#!/wiki/Wa0a1d43ca7a0_4fff_87ff_04006c762969/page/Exposing%20YOUR%20Service%20with%20ISTIO%20service)
* [Documentation](https://apps.na.collabserv.com/wikis/home?lang=en-us#!/wiki/Wa0a1d43ca7a0_4fff_87ff_04006c762969/page/Multi-tenant%20Exposing%20Service%20with%20ISTIO)
