# Utiliser l'image officielle de Node.js basée sur Alpine Linux, version 20.
FROM node:20-alpine
# Définir le répertoire de travail dans le conteneur.
WORKDIR /app
# Copier les fichiers package.json et package-lock.json dans le répertoire de travail.
COPY package.json /app
# Installer les dépendances définies dans package.json.
RUN npm install 
# Copier tous les fichiers et répertoires du répertoire courant de l'hôte
COPY ./ /app/
# Indiquer que le conteneur écoute sur le port 5173.
EXPOSE 5173
# Définir la commande à exécuter lorsque le conteneur démarre.
CMD npm run dev


