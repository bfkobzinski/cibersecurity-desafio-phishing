# Phishing para captura de senhas do Facebook

## Introdução
Este desafio consiste em criar uma página falsa do Facebook para coleta de credenciais de usuários através de ataques de phishing.
Após o usuário inserir as suas credenciais na página falsa, será redirecionado para página real da aplicação com a intensão de "enganar" o usuário, evintando perceber que estava em uma página falsa.
As credenciais capturadas estarão disponíveis nos host onde o site falso está hospedado, para isso, será utilizado o setoolkit disponível no Kali Linux.

### Ferramentas necessárias
- Kali Linux
- setoolkit

### Configurando o Phishing no Kali Linux
- Necessário acesso root no via terminal: Para elevar a permissão para root, executar o comando``` sudo su ```
  ![image](https://github.com/user-attachments/assets/ef35eda1-2584-450f-907a-15cb3541ecdd)
- Iniciar a ferramenta setoolkit: executar o comando ``` setoolkit ```
  ![image](https://github.com/user-attachments/assets/71da3928-edb4-4ed4-bef9-c47505f81820)
- Selecionar o tipo de ataque: Iremos utilizar a opção 1 ``` Social-Engineering Attacks ```
  ![image](https://github.com/user-attachments/assets/4d40fce0-3ab0-4c1b-b193-04f227d67c6c)
- Selecionar o vetor de ataque: Iremos utilizar a opção 2 ``` Web Site Attack Vectors ```
  ![image](https://github.com/user-attachments/assets/35fec53f-73b5-4265-8804-0ccdbce6aa6b)
- Método de ataque: Selecionar a opção 3 ```Credential Harvester Attack Method ```
  ![image](https://github.com/user-attachments/assets/fdde5b1d-e596-4926-8816-6c7377d4ba8e)
- Método de ataque: Selecionar a opção 2 ``` Site Cloner ```
  ![image](https://github.com/user-attachments/assets/bf5a2e90-e3a6-4eec-a88c-9628e4f0ddf5)
- Será solicitado o IP onde o site falso ficará em execução, informar o IP de seu host Kali Linux
  Para obter o endereço da máquina, executar o comando ``` ifconfig ``` em um novo terminal
  Após a confirmação, volte ao terminal onde está em execução o setoolkit e valide a informação do IP apresentada, caso necessário, digite o IP correto.
  ![image](https://github.com/user-attachments/assets/cc0ea8e9-4f1f-41d7-9220-689e69a49b57)
- Informar a URL para clone: http://www.facebook.com
  ![image](https://github.com/user-attachments/assets/fd2b333c-4874-4a86-bbdf-78ff20c45350)
  


### Resutados

- Setoolkit em execução após procedimento de configuração - clone do site
  ![image](https://github.com/user-attachments/assets/46dc007a-9abc-43b3-9a09-38c1551850fa)
- Acessando a página falsa
  ![image](https://github.com/user-attachments/assets/7d83c479-08d4-4118-8e73-d1c7b356e639)
- Coletando credenciais inseridas na página falsa nas logs do setoolkit
  ![image](https://github.com/user-attachments/assets/d739c367-41d2-42cf-b6d1-936f67f8d442)

