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

- Test some code and check if LLM is working fine e.g. "Preparing environment.ipynb"

#### Running Elasticsearch
```bash
docker run -it \
    --rm \
    --name elasticsearch \
    -m 4GB \
    -p 9200:9200 \
    -p 9300:9300 \
    -e "discovery.type=single-node" \
    -e "xpack.security.enabled=false" \
    docker.elastic.co/elasticsearch/elasticsearch:8.4.3
```

Test after running:

```bash
curl http://localhost:9200
```

For reference: RAG Workshop https://github.com/alexeygrigorev/llm-rag-workshop?tab=readme-ov-file 

For instructions: https://github.com/DataTalksClub/llm-zoomcamp/tree/main/01-intro 