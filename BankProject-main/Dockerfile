# Usar imagem base com JDK
FROM openjdk:17-slim

# Criar diretório para o app
WORKDIR /app

# Copiar os arquivos do projeto
COPY . .

# Compilar os arquivos Java
RUN javac -d out $(find src -name "*.java")


# Definir o ponto de entrada
CMD ["java", "-cp", "out", "Terminal.Main"]

