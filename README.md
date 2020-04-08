# Docker Demo
Um nach git clone Submodule zu installieren: 

```shell
git submodule init
git submodule update
```

Die docker-compose.yaml startet eine dev-Umgebung, d.h.:
- Autoreload für Codeänderungen an Client und Server
- die Anwendung kommuniziert nicht innerhalb eines Docker-Networks, sondern über die Hostmaschine
