# Gerenciando-Instancias-EC2-na-AWS
Primeiro lab DIO Code Girls

💥Criação e uso de imagens AMI💥

O que é?

Na Amazon EC2, uma AMI (Amazon Machine Image) é uma imagem de máquina virtual pré-configurada, que inclui as informações necessárias para iniciar uma instância, como o sistema operativo, o servidor de aplicações e as aplicações. 

A partir de uma imagem base é possível criar outras instâncias. 

Principais pontos:

Criação: as AMIs podem ser criadas a partir de instâncias em execução ou paradas;

A AWS fornece uma variedade de AMIs públicas que podem ser usadas, ou você pode criar e usar suas próprias AMIs privadas para segurança e personalização;

É possível personalizar uma instância (instalar software, configurar definições) e, em seguida, criar uma AMI a partir dela;

Para executar instâncias no EC2, selecione uma AMI, ela oferece as informações necessárias para iniciar uma instância;

Existem diferentes tipos de AMIs, incluindo Amazon Linux, Windows e outros, a escolha é feita baseada nos requisitos da aplicação e do sistema.

💥Snapshot💥 - é um serviço de backup que tira uma foto do meu recurso -> EC2 é a máquina virtual -> EBS é o armazenamento em bloco, utilizado com instâncias EC2 -> S3 guarda os Snapshots.

É possível configurar a frequência em que os Snapshots são tirados;

São armazenados em uma matriz diferente de onde estão os volumes EBS;

Podem ser armazenados em uma região remota, a fim de recuperação de desastres (DR);

São oferecidos a diferentes custos em diferentes regiões;

Usado para criar um volume do Amazon EBS, aumentar a durabilidade de dados e fornecer um mecanismo de backup e restauração para volumes do EBS.

✅EBS faz parte do modelo IAAS✅

💢No Amazon EC2, uma imagem de máquina da Amazon (AMI) faz o backup de um servidor inteiro, incluindo todos os volumes EBS anexados💢
 
💢Um snapshot é uma cópia pontual de um determinado volume. Você pode tirar snapshot de seus volumes EBS e salvá-los no armazenamento S3💢

📚É muito usual desenhar a arquitetura do sistema📚

#Vamos utilizar o Draw.io para gerar um diagrama

#Se for trabalhar com EC2 utilize o armazenamento ESB

#Se for trabalhar com S3 utilize o armazenamento Lambda Function

#RDS refere-se aos Serviços de Área de Trabalho Remota (Remote Desktop Services) da Microsoft, uma tecnologia que permite aos usuários acessar e interagir com desktops e aplicativos virtualizados em servidores remotos, utilizando o Protocolo de Área de Trabalho Remota (RDP)

O diagrama utilizando o EC2 encontra-se na pasta /images
