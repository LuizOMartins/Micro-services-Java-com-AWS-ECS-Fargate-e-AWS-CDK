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

_______________________________________________________

O que é CloudFormation:
- É um serviço da AWS que permite criar recursos de forma programática; (templates)
- Como funciona: criação de arquivo JSON ou YAML, que descreve os recursos que serão criados;
Stacks: recursos criados pelo CloudFormation;
Eventos: cadas passo do processo de criação dos recursos é um evento;
Recursos: são os recursos que serão criados, como: EC2, S3, RDS, etc;
- O CloudFormation é um serviço regional, ou seja, os recursos são criados em uma região específica;
- O CloudFormation é um serviço gratuito, você paga apenas pelos recursos que serão criados;
- Parametros: são valores que podem ser passados para o CloudFormation, como: nome de usuário, senha, etc;
- Outputs: são valores que podem ser retornados pelo CloudFormation, como: URL de um site, etc;

_______________________________________________________
