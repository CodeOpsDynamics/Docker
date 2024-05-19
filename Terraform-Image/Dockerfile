FROM    alpine
WORKDIR /tmp
ARG     version=1.8.1
#ARG will be alive till built time only
ARG ARGTEST=test
#till build time
ENV ENVTEST=test2
#during and after build time

ADD     https://releases.hashicorp.com/terraform/1.8.1/terraform_${version}_linux_amd64.zip .
RUN     apk add unzip
RUN     unzip  terraform_${version}_linux_amd64.zip -d /usr/local/bin
#CMD     terraform --help
#ENTRYPOINT [ "terraform" ]