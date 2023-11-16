<h1>Kubernetes</h1>

<h3>Comandos en Kubernetes</h3>

<ul>
  <li>Información del Clúster</li>
  <ul>
    <li><b>kubectl get nodes</b> Listar nodos del clúster.</li>
    <li><b>kubectl describe node NOMBRE_DEL_NODO</b> Describe un nodo específico.</li>
  </ul>
  <li>Trabajo con Pods</li>
  <ul>
    <li><b>kubectl run NOMBRE_POD --image=IMAGEN</b> Crear un pod.</li>
    <li><b>kubectl get pods</b> Listar pods.</li>
    <li><b>kubectl describe pod NOMBRE_DEL_POD</b> Describe el pod.</li>
    <li><b>kubectl logs NOMBRE_dEL_POD</b> Obtener logs de un pod.</li>
    <li><b>kubectl exec -it NOMBRE_DEL_POD -- COMANDO</b> Ejecutar un comando en un pod.</li>
  </ul>
  <li>Despliegues</li>
  <ul>
    <li><b>kubectl create deployment NOMBRE --image=IMAGEN</b> Crear un despliegue.</li>
    <li><b>kubectl scale deployment NOMBRE --replicas=N</b> Escalar un despliegue.</li>
    <li><b>kubectl set image deployment/NOMBRE CONTAINER=IMAGEN_NUEVA</b></li>
  </ul>
  <li>Servicios</li>
  <ul>
    <li><b>kubectl expose deployment NOMBRE --port=PUERTO --target-port=PUERTO_DEL_POD --type=TIPO</b> Exponer un servicio.</li>
    <li><b>kubectl get services</b> Listar servicios.</li>
    <li><b>kubectl describe service NOMBRE_DEL_SERVICIO</b> Obtener infromación detallada de un servicio.</li>
  </ul>
  <li>Configuración y Despliegue con YAML</li>
  <ul>
    <li><b>kubectl create -f archivo.yaml</b> Crear recursos desde un archivo YAML.</li>
    <li><b>kubectl apply -f archivo.yaml</b> Actualizar recursos desde un archivo YAML.</li>
    <li><b>kubectl edit POD/DEPLOYMENT/SERVIE NOMBRE</b> Editar un recurso en vivo.</li>
  </ul>
  <li>Eliminar Recursos</li>
  <ul>
    <li><b>kubectl delete POD/DEPLOYMENT/SERVICE NOMBRE</b> Eliminar un recurso.</li>
    <li><b>kubectl delete -all pods/deployment/services -n NAMESPACE</b> Eliminar todos los recursos en un namespace.</li>
  </ul>
  <li>Supervisión y Diagnóstico</li>
  <ul>
    <li><b>kubectl get events</b> Obtener eventos del clúster.</li>
    <li><b>kubectl top nodes</b> Supervisar el uso de recursos en los nodos.</li>
    <li><b>kubectl top nodes</b> Supervisar el uso de recursos en los pods.</li>
  </ul>
  <li>Otros Recursos</li>
  <ul>
    <li><b>kubectl get configmap</b> Trabajar con ConfigMaps.</li>
    <li><b>kubectl get secrets</b> Trabajar con Secrets.</li>
    <li><b>kubectl get pv</b> Trabajar con Persistent Volumes.</li>
    <li><b>kubectl get pvc</b> Trabajar con Persistent Volume Claims.</li>
    <li><b>kubectl get ingress</b> Trabajar con Ingress</li>
  </ul>