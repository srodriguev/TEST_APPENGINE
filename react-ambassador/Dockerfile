# Usa una imagen base de Node.js
FROM node:14-alpine

# Establece el directorio de trabajo dentro del contenedor
WORKDIR /app

# Copia el package.json y el package-lock.json (si existe)
COPY package*.json ./

# Instala las dependencias
RUN npm install

# Copia el código de la aplicación al contenedor
COPY . .

# Expone el puerto 3000 para que pueda ser accesible desde fuera del contenedor
EXPOSE 3000

# Comando para ejecutar la aplicación
CMD ["npm", "start"]
