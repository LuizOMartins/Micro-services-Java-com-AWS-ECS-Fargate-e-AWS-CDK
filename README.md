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

Quando apagar uma Stack?
- Todos os seus recursos são apagados;

_______________________________________________________


AWS: usuario: aws-cdk
Acess Key: AKIAZWPSDCXEWYHRSJB7
Secret access key: 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

Amazon EC2: 
-   É um serviço que permite criar servidores na AWS;
-  É possível escolher o sistema operacional, como: Linux, Windows, etc;

Amazon VPC:  permite criar uma rede virtual na AWS;;
- É uma rede isolada, onde podemos criar recursos, como: EC2, RDS, etc;
- É possível criar sub-redes, rotas, gateways, etc;
- É possível conectar a VPC com a rede local, através de VPN;


Amazon ECS: permite criar e gerenciar containers na AWS;
- É possível criar clusters, serviços, tarefas, etc;

AWS Fargate: permite executar containers sem a necessidade de gerenciar servidores;

Cluster: é um grupo de servidores que executam containers;
- É possível ter vários serviços em um cluster;

Service: é um grupo de tarefas que executam o mesmo container;

Auto Scaling: permite aumentar ou diminuir a quantidade de containers, de acordo com a demanda;


Loade Balancer: permite distribuir a carga entre os containers;


_______________________________________________________

comandos:

cdk list: lista as Stack criadas;
cdk bootstrap: cria um bucket na AWS, para armazenar os arquivos do CloudFormation;
cdk diff: mostra as diferenças entre o código e o que está rodando na AWS;
