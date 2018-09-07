# rancher-chart

## Exercise

### Build jenkins image
* Clone `git clone https://github.com/FuriKuri/jenkins-lab`
* Build docker image `docker build -t <your github account>/jenkins:2.140`
* Push image `docker push <your github account>/jenkins:2.140`

### Prepare chart
* Fork repostiory `https://github.com/FuriKuri/rancher-chart`
* Replace the todos `grep -r "TODO:" .` 
* Add missing rancher files `app-readme.md` and `values.yaml` [Rancher Doc](https://rancher.com/docs/rancher/v2.x/en/catalog/custom/)
 * Add question for using a default image or a specific image and tag
 * Add question for the 'Hello World' text
 * Add question for persistence
 * Add question to which service type
  * Do not show service type question if ingress is enabled

### Start jenkins
* Add custom catalog as in rancher
* Start your jenkins over the catalog view

### Optional
* Add configurable liveness / readiness probe
* Use a StatefulSet instead of a deployment