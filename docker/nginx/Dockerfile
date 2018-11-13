FROM nginx:latest
COPY wordpress.conf /etc/nginx/conf.d/default.conf
# forward request and error logs to docker log collector
RUN adduser wordpress && \
apt-get update && \
apt-get install nano -y && \
echo 'cd /var/www/html' >> /home/wordpress/.bashrc && \
echo 'su - wordpress' >> /root/.bashrc
