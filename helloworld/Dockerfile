FROM dotnetbase

RUN mkdir helloworld

WORKDIR helloworld

RUN scl enable rh-dotnet-core10 -- dotnet new

RUN scl enable rh-dotnet-core10 -- dotnet restore

RUN scl enable rh-dotnet-core10 -- dotnet build

ENTRYPOINT ["scl", "enable", "rh-dotnet-core10", "--", "dotnet",  "run"]


