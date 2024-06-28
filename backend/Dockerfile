# Nutze ein Node.js-Image als Basis
FROM node:14

# Setze das Arbeitsverzeichnis im Container
WORKDIR /usr/src/app

# Kopiere package.json und package-lock.json
COPY package*.json ./

# Installiere die Abhängigkeiten
RUN npm install

# Kopiere den Rest des Anwendungsquellcodes
COPY . .

# Der Port, auf dem die App läuft
EXPOSE 5000

# Starte die Anwendung
CMD ["node", "server.js"]
