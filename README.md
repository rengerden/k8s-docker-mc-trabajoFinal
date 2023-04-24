# k8s-docker-mc-trabajoFinal


> Trabajo Final Docker Kubernetes - Alfonso Chávez

## Condiciones


1.  Crear una imagen pública del aplicativo en Docker Registry  
2.  Crear un cluster de Kubernetes de preferencia en GKE (puede usar cualquier  
otro pero que este en la nube)  
3.  Crear un Pod simple (dentro del Namespace default) que ejecute el aplicativo  
y la base de datos MySQL realizando la comunicación por medio de localhost  
4.  Realizar pruebas de funcionamiento mediante un Pod que contenga un  
contenedor que permita hacer un curl a los métodos del aplicativo  
5.  Crear dos Namespaces llamados name1 y name2  
6.  En el Namespaces name1 realizar la siguiente implementación:  
	 - a. Crear la base de datos en un Pod
	 - b.  Crear un Service de tipo ClusterIP que permita exponer la base de datos   
	 - c.  Crear un ConfigMap que permita desacoplar la configuración del   aplicativo  
	  - d.  Crear  la  aplicación  en  un  ReplicaSet  con  2  replicas  que use  el   ConfigMap y se conecte al Service de la base de datos
	   - e. Crear un Service de tipo ClusterIP que permita exponer el aplicativo 
	   - f.  Realizar pruebas de funcionamiento mediante un Pod que contenga un   contenedor que permita hacer un curl a los métodos del aplicativo.
 7. En  el Namespaces name2 realizar la siguiente implementación:  
	- a.  Crear la base de datos en un Statefulset  
	- b.  Crear un Service  de tipo headless  que permita exponer la base de  
datos

	- c.  Crear un Secret que permita desacoplar la configuración del aplicativo  
	- d.  Crear la aplicación en un Deployment con 4 replicas que use el Secret y se conecte al Service de la base de datos  
	- e.  Crear un Service de tipo LoadBalancer que libere el aplicativo  
	- f.  Realizar las pruebas mediante Postman

### Consideraciones de entrega :
> Versionar su trabajo en un repositorio público en github que contenga dos
directorios:

- k8s: Poner aquí toda la implementación necesaria de cada punto de
trabajo divido por sub-carpetas (punto-01, punto-02, etc)

- screens: Poner aquí las evidencia en forma de imágenes de cada punto
trabajado dividido por sub-carpetas (punto-01, punto-02, etc
