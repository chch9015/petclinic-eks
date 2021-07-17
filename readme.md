this petclinic application is java project
-----------------------------------------

to build use tool called maven
petclinic will connect with the database(mysql)
database information is in pom.xml and schema.sql

build command:  mvn clean package -P MySQL

this petclinic application deployed in the kubernetes(k8s) eks(aws cluster)

we need code + dockerfile

jenkins--maven--petclinic
job:getting the war file
/var/lib/jenkins/workspace/petclinic/target



pre-req: RDS
-------------
1)create the RDS in the eks vpc
   public
   private--create the RDS in the private subnet
2) allow the RDS-SG in eks worker node-sg
3) allow the jenkins-sg in rds-sg