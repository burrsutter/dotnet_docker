FROM rhel7

MAINTAINER Burr Sutter "burrsutter@gmail.com"

RUN yum install -y tar

COPY dotnet-rpms-2016-04-07.tar .
RUN tar -xf dotnet-rpms-2016-04-07.tar -C /

WORKDIR /dotnet-rpms

RUN yum install -y ./rh-dotnet-core10-*

ENTRYPOINT ["scl", "enable", "rh-dotnet-core10", "--"]