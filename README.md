# activemq-hawtio-standalone

- Downloaded hawtio offline .war from http://hawt.io/getstarted/index.html
- Unzipped the .war file into webapps folder in activemq
- add security stuff to bin/activemq script: ACTIVEMQ_OPTS="$ACTIVEMQ_OPTS_MEMORY -Djava.util.logging.config.file=logging.properties -Dhawtio.realm=activemq -Dhawtio.role=admins
-Dhawtio.rolePrincipalClasses=org.apache.activemq.jaas.GroupPrincipal
-Djava.security.auth.login.config=$ACTIVEMQ_CONF/login.config"

Hint:

I took this guide by Dejan Bosanac:
http://activemq.2283324.n4.nabble.com/Hawto-log-in-td4673552.html

Enabling hawtio logging doesn't work as described. Added log4j.logger.io.hawt=DEBUG to log4j.properties, but nothing happens.
I still can't login at hawtio web console.
