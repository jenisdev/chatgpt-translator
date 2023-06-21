# ChatGPT Translate with python

Opentranslator is a simple command that can be used from the terminal to translate text (text plain or from a file). It uses OpenAI API to perform all operations, you can choose which ai engine to use by passing it as a parameter.

The following project was born to study OpenAI and how it works.
If you would contribute open a pull request or issue on GitHub.

### Usage

#### Required

- Python >= 3.7
- OpenAI Account


#### Input text
```
# You can save your OPENAI_API_KEY permanently in the user's environment
export OPENAI_API_KEY="${YOUR_OPENAI_API_KEY}"

pip install opentranslator

opentranslator --translate english --text "Ciao Mondo!"
```

#### Text from file

```
opentranslator --translate english --filepath examples/it.txt
```

#### Other

```
Arg -vvv: output all info with cost of request (in progress)
```

### Dev mode

1. Setup env

```
git clone this repository

cd chatgpt-translate-app

echo 'export ="${YOUR_OPENAI_API_KEY}"' > .env

chmod +x scritps/*.sh

./scripts/setup.sh

source .activate
```

2. Usage

```
python opentranslator/app.py --filepath examples/it.txt --translate english

python opentranslator/app.py --filepath examples/en.txt --translate italian

python opentranslator/app.py --text "Ciao Mondo!" --translate english
```
