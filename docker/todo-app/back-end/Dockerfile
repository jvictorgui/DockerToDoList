# Define a imagem base a ser utilizada
FROM node:16-alpine

# Define o diretório de trabalho dentro do contêiner
WORKDIR /app/back-end

# Adiciona os módulos do Node.js pré-instalados ao diretório de trabalho
ADD ./node_modules.tar.gz /app/back-end/

# Copia o restante dos arquivos da aplicação para o diretório de trabalho
COPY . /app/back-end/

# Expõe a porta 3001 para o mundo externo
EXPOSE 3001

# Define o comando de entrada como "npm"
ENTRYPOINT [ "npm" ]

# Define o comando padrão como "start"
CMD ["start"]
