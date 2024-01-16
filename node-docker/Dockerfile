# Utiliser une image de base Node.js
FROM node:12.18.1

# Créer et définir le répertoire de travail
WORKDIR /app

#Copier le fichier package.jsonet package-lock.jsondans notre répertoire de travail
COPY package.json package.json
COPY package-lock.json package-lock.json

# Copier les fichiers de l'application vers le conteneur
COPY . .

# Installer les dépendances
RUN npm install

# Exposer le port 3000
EXPOSE 3000

# Commande pour démarrer l'application
CMD ["node", "application.js"]

