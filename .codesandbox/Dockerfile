# Étape 1 : Utiliser une image Node.js officielle
FROM node:18-bullseye

# Étape 2 : Créer un répertoire pour l'application
WORKDIR /usr/src/app

# Étape 3 : Copier les fichiers nécessaires
COPY package*.json ./

# Étape 4 : Installer les dépendances
RUN npm install

# Étape 5 : Copier tout le code source
COPY . .

# Étape 6 : Exposer le port utilisé par l'application
EXPOSE 8080


# Étape 7 : Lancer l'application
CMD ["npm", "run", "dev"]
