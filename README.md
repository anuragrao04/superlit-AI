# Superlit AI

This repository is one of three repositories that make up superlit's code base. As the name suggests, it handles all files related to LLMs

## Ollama

- The files in this repository are mostly, if not all, Modelfiles made for [ollama](https://ollama.com/)
- It is a run time for running large language models locally
- You can customize these LLMs using Modelfiles.
- It sets up an API for communicating with these large language models and that's what superlit uses.

## Setup

- Install [ollama](https://ollama.com/)
- Run `ollama create superlit-AI -f Modelfile-generic`
- Go to the [backend](https://github.com/anuragrao04/superlit-backend) and [frontend](https://github.com/anuragrao04/superlit-frontend) and follow the setup instructions there
- The backend, frontend and ollama all can be running on different machines, you just have to specify the URLs of these machines in the `.env` files of backend and frontend repos

## Some Context On Other Files Present Here

- This repository has been a space for me to experiment with different LLMs and different prompts and different parameter tunes
- The other files present here had specialized system prompts for the different tasks superlit AI has to perform. However, these created different models that ollama had to load into video memory. 
- Having multiple models in video memory at the same time was not working well, so I resorted to the generic one with a system prompt built to give context of the task at hand
- The AI landscape is still very volatile and so is this repo
