
# Instalação dos softwares necessários

## Git

Clique [aqui](https://git-scm.com/downloads) para acessar a página de download

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
    - ssh-keygen -t ed25519 -C "henrique.f@etagdigital.com" (troque pelo seu email). Não é necessário alterar nada, apenas prossiga para o próximo passo (enter) até finalizar.
    - ![image](https://github.com/user-attachments/assets/1ce98afd-72ca-4a68-95a4-c05dc8d52c1a)
    - Vá para a pasta do seu usuário e acesse .ssh (no windows C:\Users\devet) e abra a pasta .ssh
      - Caso não apareça o arquivo, clique em Visualizar -> Mostrar -> Itens ocultos.
      - ![image](https://github.com/user-attachments/assets/90966463-0e6e-43db-92f4-784c4a5954ff)
    - Vá para o seu perfil do github clicando [aqui](https://github.com/settings/profile)
    - Selecione SSH and GPG Keys
      - ![image](https://github.com/user-attachments/assets/62f1fb7f-6f79-4f34-b3c1-1e9f57da3460)
    - Selecione "New SSH Key"
      - ![image](https://github.com/user-attachments/assets/9bb9241a-b1d3-4281-a5f7-0f3e4ed3c449)
    - Selecione um titulo - como "Etag digital seu nome"
      - ![image](https://github.com/user-attachments/assets/ca3aee86-1b77-4273-bb23-fa97ac50277a)
    - Na sessão "key", entre na pasta .ssh mencionada anteriormente, abra o arquivo .pub em um editor de texto, e cole seu conteúdo no github. Desta forma, o SSH está configurado, e será possível clonar repositórios privados aos quais você tem acesso.
      - ![image](https://github.com/user-attachments/assets/0d94b7cb-f039-48a8-aa3f-ece1a6fe7a2f)

## Mongo Compass

Clique [aqui](https://www.mongodb.com/try/download/compass) para acessar a página de download

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

Clique [aqui](https://www.docker.com/) para ir para o site de download

* Inicie o arquivo de instalação
* Clique em "Ok"
  - ![image](https://github.com/user-attachments/assets/abed9a88-2daa-46a5-8b7f-e67053fb3c8c)
* Após concluir, reinicie a máquina novamente
  - ![image](https://github.com/user-attachments/assets/4c97cfe6-a054-40d6-be86-e3287f6817fe)
 
