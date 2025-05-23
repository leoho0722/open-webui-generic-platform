# open-webui-generic-platform

Deploy Open WebUI Chat UI on any platform

## Prerequisites

- Docker、Docker Compose
- Ollama (**on-premise**)

## Serve

### Create a folder for the volume in the current directory

```bash
mkdir -p ./data
```

### Run the container via docker compose

```bash
docker compose up -d
```

### Access the WebUI

Open your browser and navigate to `http://localhost:3000` to access the WebUI.

### Connect to Ollama

1. Open the WebUI in your browser.
2. In the WebUI, click the Profile icon in the top right corner and go to the settings page.
3. Change to the "Admin Settings" tab.
4. Change to the "Connections" tab.
5. Enter the URL of your Ollama server in the "Ollama API" section. The default URL is `http://host.docker.internal:11434`.
6. Click the "Save" button to save the settings.
7. You should now be able to use the Ollama server with the WebUI.

### Stop the container

```bash
docker compose down
```
