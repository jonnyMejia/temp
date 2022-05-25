# Kubernetes

## ¿Que son Kubernetes?

Es una herramienta de orquestación de contenedores open-source diseñada para automatizar despliegues, escalamiento y operar aplicaciones de contenedores. 

Nace producto de una experiencia de Google el cual buscaba escalar de manera masiva la carga de trabajo.

Permite a las organizaciones incemrentar la velocidad de sus lanzamientos y recuperarlos

## Informacion Adicional

* Kubernetes es un sistema distribuidos, tanto para maquinas fisicas, virtuales, on premise o en la nube

* Se pueden calendarizar los contenedores en las maquinas

* Es posible mover los contenedores como agregar y retirar las maquinas

* Pueden utilizar diferentes runtimes en los contenedores

## Arquitectura de Kubernetes

* **Cluster**: se refiere al conjunto de maquinas que se interpreta como un solo sistema.
* **nodo**: son aquellas maquinas dentro de un cluster, pueden ser workers(Aplicacion) o master(API).
* **Workers**: Incluyen el software para correr los contenedores administrados por el panel de control de kubernetes
* **Masters**: Son nodos que corren el panel de control
* **Panel de control**: Conjunto de Apis y software que los usuarios utilizan para interactuar con los nodos
* **Panel de control**: Conjunto de Apis y software que los usuarios utilizan para interactuar con los nodos

## Scheduling

* El panel de control planifica sobre los contenedores de los nodes
* Planifica decisiones, considera requerimiento del CPU y otros factores
* Planifica se requiere al proceso de tomas de decisiones que toma lugar en cada contenedor de cada nodo.

## Pods
* Contiene un determinado grupo de contenedores
* Los pods es el concepto mas pequeño en kubernetes
* El uso mas complejo y util de abstraccion se desarrollara sobre los pods.

## Servicios

* Definen las reglas de red para exponer al grupo de pods tanto para otros pods como para internet publico.

## Deployments

* Buena practica de administrar un despliegue de configuracion de pods
* Permiten un escalamiento horizontal

## Comandos KUBECTL

* **kubectl create**: Para crear recursos
* **kubectl delete**: Para eliminar recursos
* **kubectl get**: Para listar recursos (Pods, Servicios, etc)
* **kubectl decribe**: Para describir informacion detallada del recurso
 **kubectl logs**: Para imprimir los logs del contenedor