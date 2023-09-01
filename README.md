This example JMS works with JBoss EAP 7.2.

https://developers.redhat.com/products/eap/download
<br/>
https://developers.redhat.com/content-gateway/file/jboss-eap-7.2.0.zip

Run jboss using standard-full.xml.<br/>
`./standalone.sh -c standalone-full.xml`

Add admin user.<br/>
`./add-user.sh`

Make sure to add application user.<br/>
`./add-user.sh -a -u 'jms' -p 'password' -g 'guest'`

Add jms queue.<br/>
`<jms-queue name="TestingQueue" entries="java:jboss/exported/jms/queue/TestingQueue"/>`