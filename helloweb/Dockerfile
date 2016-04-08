FROM dotnetbase

RUN mkdir /helloweb

COPY . /helloweb

WORKDIR /helloweb

RUN scl enable rh-dotnet-core10 -- dotnet restore

# RUN scl enable rh-dotnet-core10 -- dotnet build

EXPOSE 5000

ENTRYPOINT ["scl", "enable", "rh-dotnet-core10", "--", "dotnet",  "run"]


