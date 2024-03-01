# Trusted Application Pipeline Software Template

This application, **ssasd22445**, was created from a Trusted Application Pipeline Software Template.

The software templates create a new source and gitops deployment repositories with a sample source application. 

## Repositories

The source code for your application can be found in [https://github.com/stephanie-cy/ssasd22445 ](https://github.com/stephanie-cy/ssasd22445 ).
 
The gitops repository, which contains the kubernetes manifests for the application can be found in 
[https://github.com/stephanie-cy/ssasd22445-gitops ](https://github.com/stephanie-cy/ssasd22445-gitops ) 

## Application namespaces 

The default application will be found in the following namespaces. Applications can be deployed into unique namespaces or multiple software templates can also bet generated into the same group namespaces.  

|  Namespace   |  Description   |  
| -------- | -------- |   
| **ssasd22445-development** | The default application during development. Every build will be deployed to this namespace for testing. | 
| **ssasd22445-stage** | The staging namespace for this application. Promotion from development to stage is manual via an update to the [gitops repository](https://github.com/stephanie-cy/ssasd22445-gitops ) in the components/ssasd22445/overlays/prod directory |  
| **ssasd22445-prod** | The production namespace for this application. Promotion from stage to production is manual via an update to the [gitops repository](https://github.com/stephanie-cy/ssasd22445-gitops ) in the components/ssasd22445/overlays/prod directory | 