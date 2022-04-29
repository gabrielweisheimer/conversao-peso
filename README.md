# conversao-peso

## Steps:
1. docker build -t gweisheimer/conversao-peso:v1 -f Dockerfile ./ConversaoPeso.Web
2. docker push gweisheimer/conversao-peso:v1
3. docker tag gweisheimer/conversao-peso:v1 gweisheimer/conversao-peso:latest
4. docker push gweisheimer/conversao-peso:latest
5. docker run -d --name peso -p 8083:80 gweisheimer/conversao-peso:v1