# ![Icon](./.bluemix/secure-lock-kubernetes.png) Secure Kubernetes toolchain


### Continuously deliver a secure Docker app to a Kubernetes Cluster
This Hello World application uses Docker with Node.js and includes a DevOps toolchain that is preconfigured for continuous delivery with Vulnerability Advisor, source control, issue tracking, and online editing, and deployment to the IBM Bluemix Containers service.

Application code is stored in source control, along with its Dockerfile and its Kubernetes deployment script.
The target cluster is configured during toolchain setup (using a Bluemix API key and cluster name). You can later change these by altering the Delivery Pipeline configuration.
Any code change to the Git repo will automatically be built, validated and deployed into the Kubernetes cluster.

![Icon](./.bluemix/toolchain.png)

### To get started, click this button:
[![Deploy To Bluemix](https://console.bluemix.net/devops/graphics/create_toolchain_button.png)](https://console.bluemix.net/devops/setup/deploy/?repository=https%3A//github.com/mikewurtz/mts-toolchain)

---
### Learn more 

* Blog [Continuously deliver your app to Kubernetes with Bluemix](https://www.ibm.com/blogs/bluemix/2017/07/continuously-deliver-your-app-to-kubernetes-with-bluemix/)
* Step by step [tutorial](https://www.ibm.com/devops/method/tutorials/tc_secure_kube)
* **First-time IBM Container Service users**: Make sure that your container image registry is correctly set up with a [namespace](https://console.bluemix.net/docs/services/Registry/index.html).
    * IMPORTANT NOTE: For the pipeline to build containers successfully, please use these steps to define your namespace:
        * bx login
        * bx target --cf
        * bx cr namespace-add <my_namespace>
* [Getting started with Bluemix clusters](https://console.bluemix.net/docs/containers/container_index.html?pos=2)
* [Getting started with toolchains](https://bluemix.net/devops/getting-started)
* [Documentation](https://console.ng.bluemix.net/docs/services/ContinuousDelivery/index.html?pos=2)
