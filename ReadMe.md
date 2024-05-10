# Classificação de Imagens com Erros de Ortografia
Esse repositório contém códigos em Python que classifica imagens, em um bucket Google Cloud, com erros de ortografia.

# Passos necessários para execução desse script.
## Ativando Vertex API
  Em API Library, ative a Vertex API<br />
  /Ativar a API do Vertex AI no Google Cloud Plataform<br />
  Na aba "Credentials" da API, gere uma Service Account<br />
  Atrele sua conta gmail do Google Cloud e baixe o arquivo JSON<br />
  Nomeie o arquivo JSON para "vertex-key.json"<br />
  E faça upload para o COLAB

## Criando Bucket
  Criar um bucket nomeado "images_for_revision"<br />
  Criar um basta images<br />
  Dento da pasta adicionar as imagens a serem analisadas
#### Dica:
  Crie o bucket em apenas uma região: us-central1

## A nível de teste execute o comando a seguir para liberação de comunicação da API e do bucket com a aplicação COLAB
  Abra o Cloud Shell do Google Cloud<br />
  execute o comando 'gcloud auth application-default login --no-launch-browser'<br />
  Acesse o link gerado<br />
  Logue com sua conta gmail e aceite as solicitações de segurança<br />
  Um código com diversos caracteres serão apresentados<br />
  Copie e cole o código na console do gcloud

## Atualize as informações do código com as informações do seu projeto Cloud
  GOOGLE_API_KEY='API_KEY'<br />
  credentials = service_account.Credentials.from_service_account_file("/content/vertex-key.json")<br />
  project_id = "PROJECT_ID"<br />
  location="região" exemplo: us-central1
  
