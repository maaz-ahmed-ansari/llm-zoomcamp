## Prerequisite: Below applications to be installed already
- Python
- Docker

## Prepare Environment

- Install required libraries
```bash
 pip install -r requirements.txt
```
requirements.txt contain:
```
tqdm
python-dotenv
ipykernel
openai
elasticsearch
pandas
scikit-learn
python-dotenv
groq
```

- Set env variable: OPENAI_API_KEY with OPENAI API Key
```bash
 export OPENAI_API_KEY="<OPENAI API Key>"
```

- Run Jupyter Lab
```
jupyter lab
```
