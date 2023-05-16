# Micro-services-Java-com-AWS-ECS-Fargate-e-AWS-CDK

Preparação do ambiente de desenvolvimento:
Ferramentas:

_______________________________________________________



Erros comuns:
netstat -ano | findstr 8080
- fechar processo que está usando a porta 8080;


_______________________________________________________

Estratégia para rodar aplicação:

1- Gerar JAR
2 - O Jar será incluido em uma imagem Docker, contendo apenas o necessário;
3 - A imagem será enviada em um repositório Docker;


_______________________________________________________

DockerFile: instruções para montage da imagem Docker.
