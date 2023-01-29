# Voice-assisstent

An unofficial Python wrapper for OpenAI's ChatGPT API

## Getting Started

> Since version 0.3.0, this library is using only the `undetected_chromedriver` to bypass Cloudflare's anti-bot protection. `requests` module is no longer used due to the complexity of the protection. **Please make sure you have [Google Chrome](https://www.google.com/chrome/) / [Chromium](https://www.chromium.org/) before using this wrapper.**

### Installation

```bash
pip install -U pyChatGPT
```

### Usage

#### Obtaining session_token

1. Go to https://chat.openai.com/chat and open the developer tools by `F12`.
2. Find the `__Secure-next-auth.session-token` cookie in `Application` > `Storage` > `Cookies` > `https://chat.openai.com`.
3. Copy the value in the `Cookie Value` field.


#### Interactive mode

```bash
python3 -m pyChatGPT
```
### How do I get it to work on Google Colab?

It is normal for the seession to be crashed when installing dependencies. Just ignore the error and run your script.

```python
# install dependencies
!apt install chromium-browser xvfb
!pip install -U selenium_profiles pyChatGPT

# install chromedriver
from selenium_profiles.utils.installer import install_chromedriver
install_chromedriver()
```

```python
# start your script as normal
!python3 -m pyChatGPT
```

## Insipration

This project is inspired by

-   [ChatGPT](https://github.com/acheong08/ChatGPT)
-   [chatgpt-api](https://github.com/transitive-bullshit/chatgpt-api)


<img src="Screenshot 2023-01-29 131106.jpg" alt="UI" height="300" width="1000" />
