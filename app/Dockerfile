#image de base
FROM node:20-alpine

#dossier de travail
WORKDIR /app

COPY package.json ./

#installation des dépendances
RUN npm install --production

#copie du reste des fichiers
COPY . .

#exposition du port
EXPOSE 3000

#commande de démarrage
CMD ["node", "src/index.js"]
