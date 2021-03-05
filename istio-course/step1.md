`git clone https://github.com/DickChesterwood/istio-fleetman`{{execute T1}}
`cd istio-fleetman/_course_files/warmup-exercise/`{{execute T1}}
`kubectl apply -f ./1-istio-init.yaml`{{execute T1}}
`kubectl apply -f ./2-istio-minikube.yaml`{{execute T1}}
`kubectl get po -n istio-system`{{execute T1}}
`kubectl apply -f ./3-kiali-secret.yaml`{{execute T1}}
`kubectl label namespace default istio-injection=enabled`{{execute T1}}
`kubectl describe ns default`{{execute T1}}
`kubectl apply -f ./4-application-full-stack.yaml`{{execute T1}}
`kubectl get po`{{execute T1}}
https://[[HOST_SUBDOMAIN]]-30080-[[KATACODA_HOST]].environments.katacoda.com/
https://[[HOST_SUBDOMAIN]]-31546-[[KATACODA_HOST]].environments.katacoda.com/