# fluxcd-cloudcamp

Instalar FluxCD:
brew install fluxcd/tap/flux

Crear llave SSH:
ssh-keygen
-m PEM
-t rsa
-b 4096
-C "user@mail.com"
-f /Users/hocknas/Documents/CLOUDCAMP/septiembre-flux

Installar FluxCD en el Cluster

flux bootstrap git --url=ssh://git@github.com/Arkhantos/fluxcd-cloudcamp --branch=main --private-key-file=/mnt/shared/_CloudCamp-k8s/key-flux --path=clusters/cloducamp --context=vcc-eksctl.us-east-1.eksctl.io
