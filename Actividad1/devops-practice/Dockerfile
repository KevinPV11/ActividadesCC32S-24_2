#Usa la imagen oficial de Node.js
FROM node:14

#Establece el directorio de trabajo en el contenedor
WORKDIR /app

#Copia los archivos package.json y package-lock.json
COPY package*.json ./

#Instala las dependencias
RUN npm install

#Copia el resto de los archivos de la aplicacion
COPY . .

#Expone el puerto en el que la aplicacion correra
EXPOSE 3001

#Establece una variable de entorno para el puerto
ENV PORT=3001

#Comando para iniciar la aplicacion
CMD ["node", "src/app.js"]
