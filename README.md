# Delegation-Admin
Script para delegar permisos de administrador a una cuenta estándar

## Documentacion
- /opt/zimbra/docs/*  (/opt/zimbra/docs/rights.txt | /opt/zimbra/docs/delegatedadmin.txt)
- https://github.com/Zimbra/adminguide/blob/master/delegatedadmin.adoc#manage-zimlets
- zmprov gar -c ALL


### [Ver permisos](https://wiki.zimbra.com/wiki/UmaT-Implementing-Delegated-Administration)
~~~
zmprov gg -g usr admin@domain.com | grep ^global | awk '{print $1,$3,$5,$6}'
zmprov gg -g usr admin@domain.com | grep ^domain | awk '{print $1,$3,$4,$6,$7}'
~~~

## Ejecucion
~~~
./delegation.sh param1 param2
param1: Dominio a modificar
param2: Correo al que se brindara los permisos de administrador

Ejemplo:
./delegation.sh domain.com new-admin@domain.com
~~~
