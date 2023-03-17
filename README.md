# IBM APP Connect Enterprise Workshop

## * Documentación URL

https://www.ibm.com/docs/en/cloud-paks/cp-integration/2022.4?topic=installing

https://www.ibm.com/docs/en/app-connect/containers_cd?topic=operator-installing-red-hat-openshift

https://www.ibm.com/docs/en/app-connect/containers_cd?topic=operator-installing-kubernetes

## * Copia de bar file Repo Server

1.- Obtener la clave ssh del directorio files de este repositorio

2.- `#chmod 400 id_rsa`

3.- `#scp -i id_rsa root@169.63.186.109:/var/www/html/mybars`

## * Bars Repo URL

https://169.63.186.109/mybars

***

## * Pasos Generales Kubernetes
El paso de la preparación de la máquina para la instalación de OLM ya fue realizado
![ws1](https://github.com/fxnaranjo/k8srhocp/raw/main/images/pasosWorkshop1.png "ws1")


***

## * Pasos Generales Openshift
Para Openshift todas las configuraciones se realizan utilizando la consola web

![ws1](https://github.com/fxnaranjo/k8srhocp/raw/main/images/pasosWorkshop2.png "ws1")


## * Container Registry Key
`#oc create secret docker-registry ibm-entitlement-key --docker-username=cp --docker-password=eyJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJJQk0gTWFya2V0cGxhY2UiLCJpYXQiOjE1Nzg2ODgyNTksImp0aSI6IjdmYmZiMTM3NGFlNTQyOWZhOTM2MDdlOGUwYTcyNDU5In0.sd_sOTRpEsR3u9cxV_rR4jsxq4tuN6YHcyVmE8AngcQ --docker-server=cp.icr.io -n <namespace>`

`#kubectl create secret docker-registry ibm-entitlement-key --docker-username=cp --docker-password=eyJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJJQk0gTWFya2V0cGxhY2UiLCJpYXQiOjE1Nzg2ODgyNTksImp0aSI6IjdmYmZiMTM3NGFlNTQyOWZhOTM2MDdlOGUwYTcyNDU5In0.sd_sOTRpEsR3u9cxV_rR4jsxq4tuN6YHcyVmE8AngcQ --docker-server=cp.icr.io -n <namespace>`


