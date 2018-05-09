FROM winstonpro/vps:basic
COPY install-ubuntu.sh /root/install-ubuntu.sh
RUN apt-get update -y && \
bash install-ubuntu.sh && \
apt-get clean && \
rm -rf /var/lib/apt/lists/* /usr/sbin/entrypoint.sh
ADD entrypoint.sh /usr/sbin
