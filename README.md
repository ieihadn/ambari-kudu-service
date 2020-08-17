# ambari-kudu-service

#Ambari集成kudu服务

# 下载ambari kudu 服务目录
VERSION=`hdp-select status hadoop-client | sed 's/hadoop-client - \([0-9]\.[0-9]\).*/\1/'`

sudo git clone https://github.com/ieihadn/ambari-kudu-service.git   /var/lib/ambari-server/resources/stacks/HDP/$VERSION/services/KUDU

# 启动Ambari
ambari-server restart



