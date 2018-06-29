FROM docker.io/busybox:latest 
RUN mkdir app
ADD /target/dubbo-demo-provider-2.5.7-assembly.tar.gz /app 
##RUN cp -rf dubbo-demo-provider-2.5.7/bin/ /app 
##RUN cp -rf dubbo-demo-provider-2.5.7/conf/ /app 
##RUN cp -rf dubbo-demo-provider-2.5.7/lib/ /app 
COPY start-docker.sh /app/bin 
RUN chmod 777 /app/bin/start-docker.sh 
CMD "tail" "-f" "/dev/null"
