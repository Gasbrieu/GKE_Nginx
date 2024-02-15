"Hello World!" hospedado em um endereço web externo com o uso de pipeline CI/CD e NGINX.

Acesso externo a aplicação: http://35.247.231.37.nip.io/

Tecnologias utilizadas:
  Docker - Utilizei o docker para gerar uma imagem python possibilitando rodar o programa no cluster Kubernetes,
  Python - Através da lib Flask e Gunicorn foi criado uma aplicação web simples retornando “Hello World!”,
  Cloud Build - Utilizei arquivos yaml para configuração da imagem Docker através do Cloud Build para facilitar na atualização do projeto hospedado no GitHub,
  Cloud Deploy (CI/CD) - Criei um pipeline de entrega contínua no Cloud Deploy utilizando dois clusters Kubernetes (Staging e Production),
  Kubernetes - Criei dois cluster Kubernetes para utilizar no pipeline de CI/CD,
  Nginx - Utilizei para gerenciar o tráfego no Cluster Kubernetes de VPC Privado;
  Artifact Registry - Para armazenar a imagem Docker utilizada no projeto
