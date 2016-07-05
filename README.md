# activemq-hawtio-standalone

- Downloaded hawtio offline .war from http://hawt.io/getstarted/index.html
- Unzipped the .war file into webapps folder in activemq
- add security stuff to bin/activemq script: ACTIVEMQ_OPTS="$ACTIVEMQ_OPTS_MEMORY -Djava.util.logging.config.file=logging.properties -Dhawtio.realm=activemq -Dhawtio.role=admins
-Dhawtio.rolePrincipalClasses=org.apache.activemq.jaas.GroupPrincipal
-Djava.security.auth.login.config=$ACTIVEMQ_CONF/login.config"
