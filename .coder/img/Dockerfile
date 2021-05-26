# See our guides for writing custom images:
# https://coder.com/docs/guides/customization

FROM codercom/enterprise-base:ubuntu

# Install programs
# RUN apt-get update && apt-get install -y ...

USER root
COPY ./initial-home/ /etc/initial-home/
RUN chown coder:coder /etc/initial-home
USER coder