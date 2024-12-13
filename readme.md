# k8s-rabbitmq

Que haremos?

1. Configuración cluser Kind
2. Erlang Cookie como secreto
3. Namespace y RBAC (Role Based Access Control)
4. Stateful Set
5. Servicio
6. Conclusiones y siguientes pasos

# Just Run

#### Descarga los fuentes

    git clone

#### Crea el cluster

    kind create cluster --config cluster-setup/rabbit.yaml

#### Despliega el cluster

    kubectl apply -k rabbitmq

Listo! ya puedes ir a la interfaz de administración de rabbit en http://localhost:15672

_Recuerda que las contraseñas están incluidas en el Stateful Set como variables de entorno_
