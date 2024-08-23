# BentoChatTTS

[ChatTTS](https://github.com/2noise/ChatTTS) is a text-to-speech model designed specifically for dialogue scenario such as LLM assistant. 

## Install Dependencies

```
git clone https://github.com/bentoml/BentoChatTTS.git
cd BentoChatTTS

# Recommend Python 3.11
pip install bentoml
pip install -r requirements.txt
```

If not already present, you need to install `libsox-dev` with your package manager first.

## Run

Start a Bento server with ChatTTS.

```
export CHAT_TTS_REPO=https://github.com/2noise/ChatTTS.git
bentoml serve
```

The server is now active at [http://localhost:3000](http://localhost:3000/). You can interact with it using the Swagger UI.

## Deploy

You can deploy the ChatTTS Bento service to BentoCloud.

[Sign up](https://www.bentoml.com/) if you haven't got a BentoCloud account.

Make sure you have [logged in to BentoCloud](https://docs.bentoml.com/en/latest/bentocloud/how-tos/manage-access-token.html), then run the following command to deploy it.

```bash
bentoml deploy .
```
