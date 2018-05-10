FROM winstonpro/vps:basic
COPY install-ubuntu.sh /root/install-ubuntu.sh
RUN sed 'N;12i service bt start' /usr/sbin/entrypoint.sh && \
apt-get update -y && \
bash install-ubuntu.sh && \
apt-get clean && \
rm -rf /var/lib/apt/lists/*
