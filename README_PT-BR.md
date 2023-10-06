[![en](https://img.shields.io/badge/lang-en-green.svg)](https://github.com/zSalocin/PB_Compass_Projeto_Final_Arquitetura/blob/main/README.md)   [![pt-br](https://img.shields.io/badge/lang-pt--br-red.svg)](https://github.com/zSalocin/PB_Compass_Projeto_Final_Arquitetura/blob/main/README_PT-BR.md)

# Cloud: Projeto-final-do-PB
AWS - Cloud Pratictioner - PB Aws - IF Fluminense - IFMT - UTFPR - UNAMA  | Programa de Bolsas - DevSecOps

#### Membros da Equipe:
- [Bruno Garcia Nazareth](https://github.com/brunoshure)
- [Nicolas Meirelles Grisostolo](https://github.com/zSalocin)
- [Raphael Antunes Marinho de Souza](https://github.com/RaphaelAntunesMarinhoDeSouza)

### Caso:
A "Fast Engineering S/A" está em busca de uma solução por parte da empresa terceira "TI SOLUÇÕES INCRÍVEIS". O eCommerce da Fast Engineering está experimentando um crescimento significativo e a solução atual não está mais conseguindo lidar com a alta demanda de acessos e compras que está enfrentando. Desde o início do ano, os acessos e as compras têm apresentado um aumento de 20% a cada mês.

**Arquitetura Atual**
* 01 servidor para Banco de Dados Mysql;
* 01 servidor para a aplicação utilizando REACT;
* 01 servidor de web Server e que armazena estáticos como fotos e links.

**Requerimentos do Pedido**
- Escopo.
- Arquitetura da Nova Solução.
- Valores.
- Prazo de Entrega.
- Cronograma Macro de Entregas.

Sobre a construção da arquitetura para o futuro website da nossa empresa, é necessario seguir as melhores práticas DevOps.

**Requesitos da Nova Arquitetura**
- Ambiente Kubernetes.
- Banco de dados PaaS.
- MultiAZ.
- Segurança de backup de dados.
- Persistência dos dados.
- Balanceamento de carga com healthcheck.
- Segurança (liberar somente o necessário/mínimo acesso possível).
  
Objetivo: Monte a proposta e a arquitetura do que a equipe propõe entregar.

___

## Projeto de Migração para a AWS - Fast Engineering S/A

## Introdução

Este repositório contém a documentação e o escopo do projeto de migração para a AWS de um e-commerce. O projeto tem como objetivo aumentar a escalabilidade e reduzir custos operacionais.

## Motivação do Cliente

A motivação por trás desta migração é a necessidade de atender à crescente demanda de acessos e compras que a Fast Engineering S/A está enfrentando.

## Escopo do Projeto

### Avaliação da Infraestrutura Atual.

![Arquitetura_Atual](https://github.com/zSalocin/PB_Compass_Projeto_Final_Arquitetura/blob/main/Assets/Arquitetura_Atual.png)

### Arquitetura da Solução Proposta:

A arquitetura proposta segue as melhores práticas e está de acordo com os pilares da AWS Well-Architected Framework.
    
  **Pilares da AWS Well-Architected Framework**
      
![Arquitetura_Atual](https://github.com/zSalocin/PB_Compass_Projeto_Final_Arquitetura/blob/main/Assets/Pilares.png)
  
  **Migração de Dados**
  
 A equipe está implementando uma migração de banco de dados crucial para o AWS RDS, adotando uma abordagem que prioriza a eficiência e a continuidade operacional. O AWS Database Migration Service (DMS) será utilizado para assegurar uma transição suave, replicando os dados de forma contínua e mantendo sua integridade. Essa estratégia tem como objetivo minimizar qualquer impacto nas operações diárias, ao mesmo tempo em que se aproveita os benefícios da escalabilidade e segurança oferecidos pela AWS. A equipe está comprometida em garantir que essa migração se concretize como uma transição tranquila e bem-sucedida.
  
  **Serviços Utilizados**
  
- **Amazon CloudFront**
  O Amazon CloudFront é um serviço de Content Delivery Network (CDN) oferecido pela Amazon Web Services (AWS). Sua principal função é acelerar a entrega de conteúdo estático e dinâmico, como páginas web, imagens, vídeos, scripts e outros arquivos multimídia, aos usuários finais com baixa latência e alta disponibilidade.
  
- **AWS Web Application Firewall (WAF)**
  - O AWS Web Application Firewall é um serviço de firewall projetado para proteger aplicações web contra ataques comuns, proporcionando proteção avançada contra ameaças, garantindo a segurança de aplicativos da web.

- **AWS Shield**
  - O AWS Shield é um serviço de segurança que protege aplicativos e recursos da AWS contra ataques DDoS (Distributed Denial of Service), fornecendo defesa contra ataques DDoS de alto nível para manter a disponibilidade dos recursos.

- **Amazon Route 53**
  - O Amazon Route 53 é um serviço DNS que permite registrar e gerenciar domínios, com roteamento de tráfego para recursos AWS, como ELB e CloudFront. Facilita o roteamento de tráfego eficiente e garante alta disponibilidade, direcionando acessos para instâncias e serviços AWS.

- **Amazon Simple Storage Service (S3)**
  - O Amazon S3 utiliza Buckets para armazenar e distribuir conteúdo estático, incluindo imagens, vídeos e arquivos, integrando-se ao CloudFront para uma entrega eficiente. Oferece armazenamento seguro e escalável para imagens, vídeos e arquivos.

- **Amazon EKS**
  - O Elastic Kubernetes Service atua como a base da arquitetura, oferecendo orquestração de contêineres por meio do Kubernetes. Proporciona orquestração de contêineres escalável, permitindo a expansão dinâmica e alta disponibilidade da aplicação.

- **Amazon Virtual Private Cloud (VPC)**
  - O Virtual Private Cloud isola a infraestrutura na nuvem e fornece controle granular sobre a rede, criando uma rede privada virtual. Cria uma rede VPC, melhorando o controle de tráfego e a segurança da infraestrutura.

- **Amazon RDS** 
  -O Amazon RDS (Relational Database Service) é um serviço de banco de dados relacional oferecido pela Amazon Web Services (AWS). Ele foi projetado para simplificar a administração, operação e escalabilidade de bancos de dados relacionais, permitindo que os desenvolvedores se concentrem em suas aplicações sem se preocupar com a gestão do banco de dados subjacente.

- **Elastic Load Balancing**
  - O Elastic Load Balancing é um serviço que distribui o tráfego entre várias instâncias ou recursos para garantir a alta disponibilidade e a escalabilidade de aplicativos.

- **Amazon CloudWatch**
  - O Amazon CloudWatch é um serviço de monitoramento e observação que fornece insights sobre o desempenho dos recursos e aplicativos AWS.

- **AWS Database Migration Service**
  - O AWS Database Migration Service facilita a migração de bancos de dados para a AWS com segurança e facilidade.

- **Amazon Cognito**
  - O Amazon Cognito é um serviço de autenticação e autorização que permite que você adicione facilmente autenticação para aplicativos da web e móveis.

- **AWS Lambda**
  - O AWS Lambda é um serviço de computação serverless que permite que você execute código sem provisionar ou gerenciar servidores.

- **AWS CloudTrail**
  - O AWS CloudTrail é um serviço que registra atividades na sua conta da AWS, permitindo auditoria e rastreamento de ações.

- **AWS CodeBuild**
  - O AWS CodeBuild é um serviço de compilação totalmente gerenciado que compila código fonte, executa testes e cria artefatos.

- **AWS CodePipeline**
  - O AWS CodePipeline é um serviço de entrega contínua que automatiza a construção, teste e implantação de aplicativos.

- **AWS CodeDeploy**
  - O AWS CodeDeploy é um serviço de implantação automatizada que facilita a implantação de aplicativos na AWS.

- **Amazon EC2**
  - O Amazon EC2 fornece instâncias virtuais sob demanda com configuração personalizável para uma ampla variedade de cargas de trabalho. Escalabilidade sob demanda, permitindo a adaptação rápida às necessidades de computação, sem investimentos antecipados em hardware físico.

- **AWS Backup**
  - O AWS Backup é um serviço de backup totalmente gerenciado que ajuda a simplificar a proteção de dados e a recuperação de recursos da AWS.

- **Cost Usage e Report**
  - O serviço de Cost Usage e Report da AWS permite rastrear e analisar o uso e os custos dos recursos da AWS.

- **Cost Explorer**
  - O Cost Explorer é uma ferramenta de análise de custos que ajuda a visualizar e entender seus gastos na AWS.

- **CloudFormation**
  - O AWS CloudFormation é um serviço que permite criar e gerenciar recursos da AWS por meio de modelos de infraestrutura como código.
 
  **Nova Arquitetura**
  
![PROJECT_ARCHITECTURE](https://github.com/zSalocin/PB_Compass_Projeto_Final_Arquitetura/blob/main/Assets/Arquitetura.jpeg)

### Valores

**Calculadora AWS** 

Acesso a [caluladora de preços da AWS](https://calculator.aws/#/)

[Estimativa da Nova Arquitetura](https://calculator.aws/#/estimate?id=f0691a4bdf6209114ce6b6391e274d6b089bec07)

![Estimativa](https://github.com/zSalocin/PB_Compass_Projeto_Final_Arquitetura/blob/main/Assets/Estimativa.png)

**Custos**

|             Item                   |                     Descrição                      |       Preço      |
|------------------------------------|----------------------------------------------------|----------------  |
| Migração Para a AWS                | Migração de dados on-premise para a AWS            | $496,40          |
| Infraestrutura da AWS              | Custo da Infraestrutura de serviços da AWS         | $5.373,72/Mensal |
| Custo da Equipe                    | Suporte e manutenção técnica                       | $3.457,76/Mensal |

### Prazo de Entrega

+ Implementação da arquitetura: **22 dias úteis**.

Equipe de 3 pessoas:
  - Trabalhando 8 horas por dia
  - Ao longo de 22 dias úteis
  - Total de 528 horas para a entrega

### Cronograma Macro de Entregas

![Cronograma](https://github.com/zSalocin/PB_Compass_Projeto_Final_Arquitetura/blob/main/Assets/Cronograma.png)