# argocd-setup
steps for argocd installation


kubectl apply -n argocd -f 
https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml

kubectl get pod -n argocd -w

kubectl get svc

kubectl get svc -n argocd

kubectl edit svc argocd-server -n argocd

minikube service list -n argocd

minikube service argocd-server -n argocd

kubectl port-forward service/argocd-server -n argocd --address 0.0.0.0 8082:443

link to follow: https://argo-cd.readthedocs.io/en/stable/getting_started/


kubectl get secret -n argocd

kubectl edit argocd-initial-admin-secret -n argocd

echo SEtiMktodzlGMEp6d2xDaw== | base64 --decode
