`git clone https://github.com/DickChesterwood/istio-fleetman`{{execute T1}}

`cd icd istio-fleetman/_course_files/1\ Telemetry/`{{execute T1}}

`kubectl apply -f ./1-istio-init.yaml`{{execute T1}}

`kubectl apply -f ./2-istio-minikube.yaml`{{execute T1}}

`kubectl get po -n istio-system`{{execute T1}}

`kubectl apply -f ./3-kiali-secret.yaml`{{execute T1}}

`kubectl apply -f ./4-label-default-namespace.yaml`{{execute T1}}

`kubectl describe ns default`{{execute T1}}

`kubectl apply -f ./5-application-no-istio.yaml`{{execute T1}}

`kubectl get po`{{execute T1}}

Web app - https://[[HOST_SUBDOMAIN]]-30080-[[KATACODA_HOST]].environments.katacoda.com/

Kiali - https://[[HOST_SUBDOMAIN]]-31000-[[KATACODA_HOST]].environments.katacoda.com/

Jaeger - https://[[HOST_SUBDOMAIN]]-31001-[[KATACODA_HOST]].environments.katacoda.com/