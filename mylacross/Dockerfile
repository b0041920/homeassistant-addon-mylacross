FROM homeassistant/amd64-base:latest

# Installiere benötigte Pakete
RUN apk add --no-cache python3 py3-pip

# Installiere mylacross (stelle sicher, dass mylacross über pip verfügbar ist oder passe den Installationsbefehl an)
RUN pip3 install mylacross

# Kopiere das Start-Skript ins Image
COPY run.sh /run.sh
RUN chmod a+x /run.sh

# Setze das Start-Kommando
CMD [ "/run.sh" ]
