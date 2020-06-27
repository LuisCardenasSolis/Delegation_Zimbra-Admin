# Delegation-Admin
Script para delegar permisos de administrador a una cuenta estándar

## Documentacion
- /opt/zimbra/docs/* | /opt/zimbra/docs/rights.txt
- https://github.com/Zimbra/adminguide/blob/master/delegatedadmin.adoc#manage-zimlets
- zmprov gar -c ALL

## Ejecucion
~~~
./delegation.sh param1 param2
param1: Dominio a modificar
param2: Correo al que se brindara los permisos de administrador

Ejemplo:
./delegation.sh domain.com new-admin@domain.com
~~~
