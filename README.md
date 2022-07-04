# Projeto - Upload/Download de Arquivos - Angular 13 + Spring-boot

# Sistema - Upload/Download de Arquivos
![1](https://user-images.githubusercontent.com/47387393/177194213-6bbea258-cb77-4fb2-ae02-299e16e93217.PNG)

# Arquitetura do Projeto
![angular-10-spring-boot-file-upload-architecture](https://user-images.githubusercontent.com/47387393/177193172-37baf510-b21b-4617-8681-61714ff648a3.png)

## Angular Client
  - O componente FileUpload chama as funções UploadService para arquivos de upload/download/exibição
  - UploadService usa HttpClientModule para fazer solicitações HTTP
  
## Servidor Spring
  - FilesController recebe as requisições HTTP do Cliente, então chama Funções FilesStorageService para upload/download/obtenção de arquivos
  - FilesStorageService implementa funções para armazenar e recuperar sistemas de arquivos usando a biblioteca Java Files
