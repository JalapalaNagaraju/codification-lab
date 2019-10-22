In this step we will install check the minikube version installed on the system
`minikube version`{{execute}}

Download Labs
`git clone https://github.com/JalapalaNagaraju/amazic-workshop.git`{{execute}}

Lab1
`cd amazic-workshop/Lab1`{{execute}}

Download Istio
`curl -L https://git.io/getLatestIstio | ISTIO_VERSION=1.3.3 sh -`{{execute}}
`cd istio-1.3.3/`{{execute}}
`export PATH=$PWD/bin:$PATH`{{execute}}
`for i in install/kubernetes/helm/istio-init/files/crd*yaml; do kubectl apply -f $i; done`{{execute}}
`kubectl apply -f install/kubernetes/istio-demo.yaml`{{execute}}
`kubectl get svc -n istio-system`{{execute}}
`kubectl get pods -n istio-system`{{execute}}
