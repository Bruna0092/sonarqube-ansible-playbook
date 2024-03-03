# Instale o SonarQube com Ansible ⚙️

#### EC2 ☁️
- AMI: Amazon Linux 2023
- Type: t3.small

#### RDS ☁️
- Engine: Postgres
- Version: 15.6 R1

#### Configure o IP da sua EC2 no arquivo [inventario](https://github.com/Bruna0092/sonarqube-ansible-playbook/blob/main/inventario/hosts)
#### Altere o caminho da chave .PEM
https://img.shields.io/badge/teste-8A2BE2

#### Altere as os valores das variaveis do arquivo [db_conf/vars/main.yml](https://github.com/Bruna0092/sonarqube-ansible-playbook/blob/main/roles/db_conf/vars/main.yml)

#### Execute o comando no diretorio do projeto

```sudo ansible-playbook sonarqube.yml -i inventario/hosts
```

#### Etapas:
- Pré configuração da máquina
- Download e instalação
- Criação da Database e usuario do serviço
- Pós instalação: ajuste no arquivo sonar.properties e start do serviço
