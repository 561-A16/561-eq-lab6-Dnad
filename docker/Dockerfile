FROM ymazieres/dotnet:compile

WORKDIR /src
ENV ASPNETCORE_URLS http://+:5000

CMD ["sh","/script/run.sh"]
COPY /docker/run.sh /script/run.sh
RUN chmod +x /script/run.sh

COPY /src /src 

#docker build -t webapp -f ./docker/Dockerfile .

#docker run -it --rm -v $PWD/packages:/root/.nuget/packages -p 8080:5000 webapp