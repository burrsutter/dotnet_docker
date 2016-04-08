sudo setenforce 0

docker build -t dotnetbase .
docker run -it dotnetbase bash
dotnet --help
mkdir helloworld
cd helloworld
dotnet new
dotnet restore
dotnet run


