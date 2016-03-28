FROM nuwanbando/javabase

RUN mkdir wso2 

COPY packs/wso2am-1.10.0.zip wso2/

RUN cd wso2/ && \
        unzip wso2am-1.10.0.zip

COPY artifacts/mysql-connector-java-5.1.34-bin.jar /wso2/wso2am-1.10.0/repository/components/lib/
COPY gateway/api-manager.xml /wso2/wso2am-1.10.0/repository/conf/
COPY gateway/master-datasources.xml /wso2/wso2am-1.10.0/repository/conf/datasources/
COPY gateway/registry.xml /wso2/wso2am-1.10.0/repository/conf/
COPY gateway/user-mgt.xml /wso2/wso2am-1.10.0/repository/conf/

CMD ["sh", "/wso2/wso2am-1.10.0/bin/wso2server.sh"]

EXPOSE 9763
EXPOSE 9443
EXPOSE 8280
EXPOSE 8243
EXPOSE 10397