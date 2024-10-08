
# Instalação dos softwares necessários

## Git

[Download do git](https://git-scm.com/download)

* Abra o arquivo para iniciar a instalação

* Selecione "Next" até chegar a sessão de "Choose credential helper". Nesta sessão, selecione "None", e continue selecionando next até iniciar a instalação

### Após concluir, vamos configurar seu usuário e o SSH

* Abra um terminal, como por exemplo o do próprio git
* Ao abrir, devemos configurar duas coisas: Email e Name. Isto irá servir como uma identificação para os commits feitos.
  - Nome: "git config --global user.name "Seu Nome";
    - ![image](https://github.com/user-attachments/assets/f6ca7be2-61b9-4cfb-aad5-e4a9432674b1)

  - Email: "git config --global user.email "Seu Email";
    - ![image](https://github.com/user-attachments/assets/85cc7756-151d-413b-9b98-b99ecc157e6b)
  - Para confirmar se as configurações foram feitas corretamente, você pode digitar git config --global user.name ou user.email para visualizar os dados inseridos.
    - ![image](https://github.com/user-attachments/assets/5d5e00af-2d6a-4933-87bd-e392df5c894e)
   
### Configuração do SSH
* O SSH irá servir para que você clone repositórios privados da ETag sem a necessidade de autenticação. Todas as clonagens serão feitas com SSH. Os comandos abaixo devem ser digitado em um terminal (como git bash).
    - ```ssh-keygen -t rsa-sha2-256``` . Não é necessário alterar nada, apenas prossiga para o próximo passo (enter) até finalizar.
    - ![image](https://github.com/user-attachments/assets/dbe8673c-5db5-42d4-b36a-98dd809fc91f)

    - Vá para a pasta do seu usuário e acesse .ssh (no windows C:\Users\seuUser) e abra a pasta .ssh
      - Caso não apareça o arquivo, clique em Visualizar -> Mostrar -> Itens ocultos.
      - ![image](https://github.com/user-attachments/assets/90966463-0e6e-43db-92f4-784c4a5954ff)
    - Vá para o seu perfil do azure devops clicando [aqui](https://dev.azure.com/)
    - Selecione SSH public keys
      - ![image](https://github.com/user-attachments/assets/93d53ed0-6f62-472a-a74e-a181f5ba27a8)
    - Na sessão "add", entre na pasta .ssh mencionada anteriormente, abra o arquivo id_rsa.pub em um editor de texto, e cole seu conteúdo no azure devops. Desta forma, o SSH está configurado, e será possível clonar repositórios privados aos quais você tem acesso.
      - ![image](https://github.com/user-attachments/assets/e68a935c-a63b-4dd1-a42d-198d9bb3708a)


## Mongo Compass

[Download do Mongo Compass](https://www.mongodb.com/try/download/compass)

* Após acessar a página, você terá algumas opções
  - Desça até visualizar "MongoDB Compass Download (GUI)" e faça o download.
    - ![image](https://github.com/user-attachments/assets/85308c62-d21d-457f-a495-6bbb4961008e)
  - Inicie a instalação, e ela será feita sozinha.
 
## WSL

* Abra o powershell como administrador, e insira o seguinte comando:
  - wsl --install
    - Após a conclusão, reinicie sua máquina
    - ![image](https://github.com/user-attachments/assets/302f9c74-8ddd-4c90-9fe6-f2d5d84611a4)
    - Após reiniciar, uma instalação irá se iniciar automaticamente
      - Em UNIX name, seria o seu username. Insira um de sua preferência, como seu próprio nome.
      - ![image](https://github.com/user-attachments/assets/dd55f6df-4f38-45c7-ba76-a89e97c85378)
      - E também insira uma senha que você se lembre bem
      - ![image](https://github.com/user-attachments/assets/8c75cf60-72b0-4418-b279-ee2500d7821d)

## Docker

[Download do Docker](https://www.docker.com/)

* Inicie o arquivo de instalação
* Clique em "Ok"
  - ![image](https://github.com/user-attachments/assets/abed9a88-2daa-46a5-8b7f-e67053fb3c8c)
* Após concluir, reinicie a máquina novamente
  - ![image](https://github.com/user-attachments/assets/4c97cfe6-a054-40d6-be86-e3287f6817fe)
 * Após reiniciar, docker também irá iniciar e irá te pedir para criar uma conta. É opcional
  - ![image](https://github.com/user-attachments/assets/e7fabbc4-3510-43c0-93ed-c0e5da55a812)

## DBeaver

[Download do DBEaver](https://dbeaver.io/download/)

* Selecione uma linguagem de sua preferência
  - ![image](https://github.com/user-attachments/assets/0a00f01f-e561-4bcc-a402-9b9024705937)
* Selecione "Próximo" até a instalação iniciar

## Node.Js

[Download do Node.Js](https://nodejs.org/en/download/package-manager)

* Nesta etapa, eu prefiro selecionar "Prebuilt Installer" e fazer o download do instalador
  - ![image](https://github.com/user-attachments/assets/202cc752-f095-44d1-85dc-17c82b3bf73b)
* Inicie a instalação, e clique em "próximo" até concluir.
* Para verificar se a instalação foi concluída com êxito, abra um terminal e digite "node -v". Deverá aparecer a versão do Node que foi instalada.

## Client Azure

[Download do CLI](https://learn.microsoft.com/pt-br/cli/azure/install-azure-cli-windows?tabs=azure-cli)

* Faça a instalação de sua preferência
  - Caso tenha selecionado o MSI, inicie a instalação e clique em "Next" até concluir.
* Para verificar se a instalação foi concluída, abra um terminal e digite "az -v"

### Login

* Para iniciar o processo de autenticação no Azure CLI, abra um terminal e digite "az login". Você será redirecionado para uma página para inserir suas credênciais.
  - ![image](https://github.com/user-attachments/assets/aa49f159-f76b-44f4-9c25-b52eaa0886e9)
  - Insira seu email e senha corporátivo, e conclua o Login.
