FROM microsoft/dotnet:latest
RUN mkdir /src
WORKDIR /src
ADD app/src/ /src
RUN dotnet restore
RUN dotnet build
CMD dotnet run
