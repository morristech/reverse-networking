```
PN_USER=xxx
PN_PORT=22
PN_HOST=mydomain.org
PN_VALIDATE=local # local or ssh, both requires "nc" to be installed on local or remote ($PN_HOST) machine

# optional:
#PN_VALIDATE_COMMAND="curl http://mydomain.org" # custom validation command that will be ran locally or remotely

# destination port on remote server => local port
PORTS[0]="80>8000"
PORTS[1]="2222>22"
PORTS[2]="80>8001>@gateway" # port will be available publicly
```
