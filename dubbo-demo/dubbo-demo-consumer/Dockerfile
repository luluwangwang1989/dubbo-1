FROM docker.io/busybox:latest 
 COPY /home/jenkins/workspace/dubbo-old/dubbo-demo/dubbo-demo-consumer/target/dubbo-demo-consumer-2.5.7-assembly.tar.gz / 
 RUN tar xvf dubbo-demo-consumer-2.5.7-assembly.tar.gz 
 RUN mkdir app 
RUN cp -rf dubbo-demo-consumer-2.5.7/bin/ /app 
RUN cp -rf dubbo-demo-consumer-2.5.7/lib/ /app 
RUN cp -rf dubbo-demo-consumer-2.5.7/conf/ /app 
COPY /home/jenkins/workspace/dubbo-old/dubbo-demo/dubbo-demo-consumer/start-docker.sh /app/bin
RUN chmod -R 777 /app/bin/start-docker.sh 
CMD ["sh","-c","/app/bin/start-docker.sh"]
