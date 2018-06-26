FROM docker.io/busybox:latest 
 ADD target/dubbo-demo-consumer-2.5.7-assembly.tar.gz /
 RUN mkdir app 
RUN cp -rf dubbo-demo-consumer-2.5.7/bin/ /app 
RUN cp -rf dubbo-demo-consumer-2.5.7/lib/ /app 
RUN cp -rf dubbo-demo-consumer-2.5.7/conf/ /app 
COPY start-docker.sh /app/bin
RUN chmod -R 777 /app/bin/start-docker.sh 
CMD ["sh","-c","/app/bin/start-docker.sh"]
