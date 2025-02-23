FROM homeassistant/amd64-base:latest

# Installiere Python3 und pip
RUN apk add --no-cache python3 py3-pip

# Installiere pylacrosse
RUN pip3 install pylacrosse

# Kopiere das Start-Skript ins Image
COPY run.sh /run.sh
RUN chmod a+x /run.sh

# Setze das Start-Kommando
CMD [ "/run.sh" ]
