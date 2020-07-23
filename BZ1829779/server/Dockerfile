FROM docker.io/centos:7
USER root
COPY libwebsockets/build/bin/libwebsockets-test-server /
RUN yum install -y iperf3
EXPOSE 7681 5201
CMD ["iperf3 -i 5 -s & ; /libwebsockets-test-server"]
