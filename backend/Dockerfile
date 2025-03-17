# Use uma imagem do OpenJDK para Java 17
FROM openjdk:17-jdk-slim

# Defina o diretório de trabalho no contêiner
WORKDIR /app

# Copie os arquivos do seu projeto para o contêiner
COPY ./backend /app

# Instale as dependências e construa o projeto
RUN ./mvnw clean install

# Exponha a porta 8080, que é a padrão para o Spring Boot
EXPOSE 8081

# Comando para rodar a aplicação Spring Boot
CMD ["./mvnw", "spring-boot:run"]
