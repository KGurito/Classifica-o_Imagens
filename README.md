# Classificação de Imagens com Erros de Ortografia
Esse repositório contém códigos em Python que classifica imagens, em um bucket Google Cloud, com erros de ortografia.

Passos necessários para execução desse script.
# Ativando Vertex API
  Em API Library, ative a Vertex API
  /Ativar a API do Vertex AI no Google Cloud Plataform
  Na aba "Credentials" da API, gere uma Service Account
  Atrele sua conta gmail do Google Cloud e baixe o arquivo JSON
  Nomeie o arquivo JSON para "vertex-key.json"
  E faça upload para o COLAB

# Criando Bucket
  Criar um bucket nomeado "images_for_revision"
  Criar um basta images
  Dento da pasta adicionar as imagens a serem analisadas

# A nível de teste execute o comando a seguir para liberação de comunicação da API e do bucket com a aplicação COLAB
  Abra o Cloud Shell do Google Cloud
  execute o comando 'gcloud auth application-default login --no-launch-browser'
  Acesse o link gerado
  Logue com sua conta gmail e aceite as solicitações de segurança
  Um código com diversos caracteres serão apresentados
  Copie e cole o código na console do gcloud

# Atualize as informações do código com as informações do seu projeto Cloud
  GOOGLE_API_KEY='API_KEY'
  credentials = service_account.Credentials.from_service_account_file("/content/vertex-key.json")
  project_id = "PROJECT_ID"
  location="região" exemplo: us-central1
  
