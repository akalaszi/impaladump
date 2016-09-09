# download impala jdbc driver from: http://www.cloudera.com/downloads/connectors/impala/jdbc/2-5-32.html
# unzip downloaded file and unzip Cloudera_ImpalaJDBC41_2.5.32.zip 
# add jars to local repo:
mvn install:install-file -Dfile=hive_metastore.jar -DgroupId=com.cloudera.impala.jdbc -DartifactId=hive_metastore -Dversion=2.5.32.1052 -Dpackaging=jar
mvn install:install-file -Dfile=hive_service.jar -DgroupId=com.cloudera.impala.jdbc -DartifactId=hive_service -Dversion=2.5.32.1052 -Dpackaging=jar
mvn install:install-file -Dfile=ImpalaJDBC41.jar -DgroupId=com.cloudera.impala.jdbc -DartifactId=ImpalaJDBC41 -Dversion=2.5.32.1052 -Dpackaging=jar
mvn install:install-file -Dfile=TCLIServiceClient.jar -DgroupId=com.cloudera.impala.jdbc -DartifactId=TCLIServiceClient -Dversion=2.5.32.1052 -Dpackaging=jar
mvn install:install-file -Dfile=ql.jar -DgroupId=com.cloudera.impala.jdbc -DartifactId=ql -Dversion=2.5.32.1052 -Dpackaging=jar
