<a name="readme-top"></a>

<!-- PROJECT LOGO -->
<br />
<div align="center">
  <h2>Cheshire-Cat (Stregatto)</h2>
<br/>
  <a href="https://github.com/cheshire-cat-ai/core">
  <img alt="GitHub Repo stars" src="https://img.shields.io/github/stars/cheshire-cat-ai/core?style=social">
</a>
  <a href="https://discord.gg/bHX5sNFCYU">
        <img src="https://img.shields.io/discord/1092359754917089350?logo=discord"
            alt="chat on Discord"></a>
  <a href="https://github.com/cheshire-cat-ai/core/issues">
  <img alt="GitHub issues" src="https://img.shields.io/github/issues/cheshire-cat-ai/core">
  </a>
  <a href="https://github.com/cheshire-cat-ai/core/tags">
  <img alt="GitHub tag (with filter)" src="https://img.shields.io/github/v/tag/cheshire-cat-ai/core">
  </a>
  <img alt="GitHub top language" src="https://img.shields.io/github/languages/top/cheshire-cat-ai/core">

  <br/>
  <img src="./readme/cheshire_cat_generated_mj.jpeg" alt="Logo" width="600" height="auto" alt="Image generated by Midjourney, prompted by Edgars Romanovskis">
</div>

## Production ready AI assistant framework

The Cheshire Cat is a framework to build custom AIs on top of any language model. 
If you ever used systems like WordPress or Django to build web apps, imagine the Cat as a similar tool, but specific for AI.

Why use the Cat:
- 🌍 Supports any language model (works with OpenAI chatGPT, LLAMA2, HuggingFace models, custom)
- 🐘 Rememebers conversations and documents and uses them in conversation
- 🚀 Extensible via plugins (AI can connect to your APIs or execute custom python code)
- 🐋 Production Ready - 100% [dockerized](https://docs.docker.com/get-docker/)
- 👩‍👧‍👦 Active [Discord community](https://discord.gg/bHX5sNFCYU) and easy to understand [docs](https://cheshire-cat-ai.github.io/docs/)

We are committed to openness, privacy and creativity, we want to bring AI to the long tail. If you want to know more about our vision and values, read the [Code of Ethics](./readme/CODE-OF-ETHICS.md). 

This project is growing fast, refactorings and code changes happens very often, join the [Issues](https://github.com/cheshire-cat-ai/core/issues?q=is%3Aissue+is%3Aopen+sort%3Aupdated-desc) to help!

## Docs and Resources
- [Official Documentation](https://cheshire-cat-ai.github.io/docs/)
- [Discord Server](https://discord.gg/bHX5sNFCYU)
- [Website](https://cheshirecat.ai/)
- [YouTube tutorial - How to install](https://youtu.be/Rvx19TZBCrw)
- [Tutorial - Write your first plugin](https://cheshirecat.ai/write-your-first-plugin/)

## Quickstart


### Install

To make Cheshire Cat run on your machine, you just need [`docker`](https://docs.docker.com/get-docker/) and [`docker compose`](https://docs.docker.com/compose/install/) installed.
Clone the repo: 

```bash
git clone https://github.com/cheshire-cat-ai/core.git cheshire-cat
```

Enter the created folder:

```bash
cd cheshire-cat
```

After that you can run:

```bash
docker compose up
```

The first time (only) it will take several minutes, as the images occupy a few GBs.

- Chat with the Cheshire Cat on [localhost:1865/admin](http://localhost:1865/admin).
- You can also interact via REST API and try out the endpoints on [localhost:1865/docs](http://localhost:1865/docs)

As a first thing, the Cat will ask you to configure your favourite language model.
It can be done directly via the interface in the Settings page (top right in the admin).

Enjoy the Cat!

When you're done, remember to CTRL+c in the terminal and
```
docker compose down
```

### Update

From time to time it is a good idea to update the Cat:

```
docker compose down
git pull origin main
docker compose build --no-cache
docker compose up
```

### Running Tests

To run the tests within the Docker container, execute the following command:

```bash
docker exec cheshire_cat_core python -m pytest --color=yes .
```

### Try in GitHub Codespaces

You can try Cheshire Cat in GitHub Codespaces. The free account provides 60 free hours a month.

[![Try in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/cheshire-cat-ai/core)

## Roadmap

Detailed roadmap is [here](./readme/ROADMAP.md).
Whilst for the current progress of development, take a look at the [projects](https://github.com/orgs/cheshire-cat-ai/projects) marked as open.

## Contributing

Send your pull request to the `develop` branch. Here is a [full guide to contributing](./readme/CONTRIBUTING.md).

To get started you can:
- Trying out the Cat
- Sharing on social media
- Join our [community on Discord](https://discord.gg/bHX5sNFCYU)
- Give the project a star ⭐!

Thanks again!🙏

## Credits

Logo image generated with MidJourney, prompted by [Edgars Romanovskis](https://www.linkedin.com/in/edgars-romanovskis-b28826259/)

## Which way to go?

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<p align="center">
    <img align="center" src=./readme/cheshire-cat.jpeg width=400px alt="Wikipedia picture of the Cheshire Cat">
</p>

```
"Would you tell me, please, which way I ought to go from here?"
"That depends a good deal on where you want to get to," said the Cat.
"I don't much care where--" said Alice.
"Then it doesn't matter which way you go," said the Cat.

(Alice's Adventures in Wonderland - Lewis Carroll)

```
