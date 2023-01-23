from google.colab import drive
drive.mount('/content/drive')
Mounted at /content/drive
[ ]
!pip install simpletransformers
Looking in indexes: https://pypi.org/simple, https://us-python.pkg.dev/colab-wheels/public/simple/
Collecting simpletransformers
  Downloading simpletransformers-0.63.9-py3-none-any.whl (250 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 250.5/250.5 KB 16.1 MB/s eta 0:00:00
Collecting tokenizers
  Downloading tokenizers-0.13.2-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (7.6 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 7.6/7.6 MB 93.6 MB/s eta 0:00:00
Collecting transformers>=4.6.0
  Downloading transformers-4.25.1-py3-none-any.whl (5.8 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 5.8/5.8 MB 64.6 MB/s eta 0:00:00
Requirement already satisfied: scikit-learn in /usr/local/lib/python3.8/dist-packages (from simpletransformers) (1.0.2)
Requirement already satisfied: pandas in /usr/local/lib/python3.8/dist-packages (from simpletransformers) (1.3.5)
Collecting seqeval
  Downloading seqeval-1.2.2.tar.gz (43 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 43.6/43.6 KB 5.7 MB/s eta 0:00:00
  Preparing metadata (setup.py) ... done
Requirement already satisfied: tensorboard in /usr/local/lib/python3.8/dist-packages (from simpletransformers) (2.9.1)
Collecting streamlit
  Downloading streamlit-1.17.0-py2.py3-none-any.whl (9.3 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 9.3/9.3 MB 95.7 MB/s eta 0:00:00
Requirement already satisfied: scipy in /usr/local/lib/python3.8/dist-packages (from simpletransformers) (1.7.3)
Collecting sentencepiece
  Downloading sentencepiece-0.1.97-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (1.3 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 1.3/1.3 MB 80.7 MB/s eta 0:00:00
Requirement already satisfied: numpy in /usr/local/lib/python3.8/dist-packages (from simpletransformers) (1.21.6)
Collecting datasets
  Downloading datasets-2.8.0-py3-none-any.whl (452 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 452.9/452.9 KB 44.9 MB/s eta 0:00:00
Collecting wandb>=0.10.32
  Downloading wandb-0.13.9-py2.py3-none-any.whl (2.0 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 2.0/2.0 MB 98.9 MB/s eta 0:00:00
Requirement already satisfied: tqdm>=4.47.0 in /usr/local/lib/python3.8/dist-packages (from simpletransformers) (4.64.1)
Requirement already satisfied: regex in /usr/local/lib/python3.8/dist-packages (from simpletransformers) (2022.6.2)
Requirement already satisfied: requests in /usr/local/lib/python3.8/dist-packages (from simpletransformers) (2.25.1)
Requirement already satisfied: filelock in /usr/local/lib/python3.8/dist-packages (from transformers>=4.6.0->simpletransformers) (3.9.0)
Collecting huggingface-hub<1.0,>=0.10.0
  Downloading huggingface_hub-0.11.1-py3-none-any.whl (182 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 182.4/182.4 KB 26.2 MB/s eta 0:00:00
Requirement already satisfied: packaging>=20.0 in /usr/local/lib/python3.8/dist-packages (from transformers>=4.6.0->simpletransformers) (21.3)
Requirement already satisfied: pyyaml>=5.1 in /usr/local/lib/python3.8/dist-packages (from transformers>=4.6.0->simpletransformers) (6.0)
Requirement already satisfied: typing-extensions in /usr/local/lib/python3.8/dist-packages (from wandb>=0.10.32->simpletransformers) (4.4.0)
Collecting docker-pycreds>=0.4.0
  Downloading docker_pycreds-0.4.0-py2.py3-none-any.whl (9.0 kB)
Requirement already satisfied: psutil>=5.0.0 in /usr/local/lib/python3.8/dist-packages (from wandb>=0.10.32->simpletransformers) (5.4.8)
Requirement already satisfied: setuptools in /usr/local/lib/python3.8/dist-packages (from wandb>=0.10.32->simpletransformers) (57.4.0)
Collecting sentry-sdk>=1.0.0
  Downloading sentry_sdk-1.13.0-py2.py3-none-any.whl (177 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 177.4/177.4 KB 22.4 MB/s eta 0:00:00
Collecting GitPython>=1.0.0
  Downloading GitPython-3.1.30-py3-none-any.whl (184 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 184.0/184.0 KB 23.8 MB/s eta 0:00:00
Requirement already satisfied: appdirs>=1.4.3 in /usr/local/lib/python3.8/dist-packages (from wandb>=0.10.32->simpletransformers) (1.4.4)
Collecting pathtools
  Downloading pathtools-0.1.2.tar.gz (11 kB)
  Preparing metadata (setup.py) ... done
Requirement already satisfied: Click!=8.0.0,>=7.0 in /usr/local/lib/python3.8/dist-packages (from wandb>=0.10.32->simpletransformers) (7.1.2)
Requirement already satisfied: protobuf!=4.21.0,<5,>=3.12.0 in /usr/local/lib/python3.8/dist-packages (from wandb>=0.10.32->simpletransformers) (3.19.6)
Collecting setproctitle
  Downloading setproctitle-1.3.2-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl (31 kB)
Requirement already satisfied: urllib3<1.27,>=1.21.1 in /usr/local/lib/python3.8/dist-packages (from requests->simpletransformers) (1.24.3)
Requirement already satisfied: idna<3,>=2.5 in /usr/local/lib/python3.8/dist-packages (from requests->simpletransformers) (2.10)
Requirement already satisfied: chardet<5,>=3.0.2 in /usr/local/lib/python3.8/dist-packages (from requests->simpletransformers) (4.0.0)
Requirement already satisfied: certifi>=2017.4.17 in /usr/local/lib/python3.8/dist-packages (from requests->simpletransformers) (2022.12.7)
Requirement already satisfied: fsspec[http]>=2021.11.1 in /usr/local/lib/python3.8/dist-packages (from datasets->simpletransformers) (2022.11.0)
Requirement already satisfied: pyarrow>=6.0.0 in /usr/local/lib/python3.8/dist-packages (from datasets->simpletransformers) (9.0.0)
Collecting xxhash
  Downloading xxhash-3.2.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (213 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 213.0/213.0 KB 24.1 MB/s eta 0:00:00
Requirement already satisfied: dill<0.3.7 in /usr/local/lib/python3.8/dist-packages (from datasets->simpletransformers) (0.3.6)
Collecting multiprocess
  Downloading multiprocess-0.70.14-py38-none-any.whl (132 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 132.0/132.0 KB 16.6 MB/s eta 0:00:00
Requirement already satisfied: aiohttp in /usr/local/lib/python3.8/dist-packages (from datasets->simpletransformers) (3.8.3)
Collecting responses<0.19
  Downloading responses-0.18.0-py3-none-any.whl (38 kB)
Requirement already satisfied: pytz>=2017.3 in /usr/local/lib/python3.8/dist-packages (from pandas->simpletransformers) (2022.7)
Requirement already satisfied: python-dateutil>=2.7.3 in /usr/local/lib/python3.8/dist-packages (from pandas->simpletransformers) (2.8.2)
Requirement already satisfied: threadpoolctl>=2.0.0 in /usr/local/lib/python3.8/dist-packages (from scikit-learn->simpletransformers) (3.1.0)
Requirement already satisfied: joblib>=0.11 in /usr/local/lib/python3.8/dist-packages (from scikit-learn->simpletransformers) (1.2.0)
Collecting watchdog
  Downloading watchdog-2.2.1-py3-none-manylinux2014_x86_64.whl (78 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 79.0/79.0 KB 10.8 MB/s eta 0:00:00
Requirement already satisfied: toml in /usr/local/lib/python3.8/dist-packages (from streamlit->simpletransformers) (0.10.2)
Collecting blinker>=1.0.0
  Downloading blinker-1.5-py2.py3-none-any.whl (12 kB)
Collecting semver
  Downloading semver-2.13.0-py2.py3-none-any.whl (12 kB)
Requirement already satisfied: tzlocal>=1.1 in /usr/local/lib/python3.8/dist-packages (from streamlit->simpletransformers) (1.5.1)
Requirement already satisfied: cachetools>=4.0 in /usr/local/lib/python3.8/dist-packages (from streamlit->simpletransformers) (5.2.1)
Collecting validators>=0.2
  Downloading validators-0.20.0.tar.gz (30 kB)
  Preparing metadata (setup.py) ... done
Requirement already satisfied: pillow>=6.2.0 in /usr/local/lib/python3.8/dist-packages (from streamlit->simpletransformers) (7.1.2)
Collecting pydeck>=0.1.dev5
  Downloading pydeck-0.8.0-py2.py3-none-any.whl (4.7 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 4.7/4.7 MB 111.4 MB/s eta 0:00:00
Collecting pympler>=0.9
  Downloading Pympler-1.0.1-py3-none-any.whl (164 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 164.8/164.8 KB 21.7 MB/s eta 0:00:00
Requirement already satisfied: tornado>=5.0 in /usr/local/lib/python3.8/dist-packages (from streamlit->simpletransformers) (6.0.4)
Requirement already satisfied: altair>=3.2.0 in /usr/local/lib/python3.8/dist-packages (from streamlit->simpletransformers) (4.2.0)
Requirement already satisfied: importlib-metadata>=1.4 in /usr/local/lib/python3.8/dist-packages (from streamlit->simpletransformers) (6.0.0)
Collecting rich>=10.11.0
  Downloading rich-13.2.0-py3-none-any.whl (238 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 238.9/238.9 KB 27.6 MB/s eta 0:00:00
Requirement already satisfied: wheel>=0.26 in /usr/local/lib/python3.8/dist-packages (from tensorboard->simpletransformers) (0.38.4)
Requirement already satisfied: grpcio>=1.24.3 in /usr/local/lib/python3.8/dist-packages (from tensorboard->simpletransformers) (1.51.1)
Requirement already satisfied: absl-py>=0.4 in /usr/local/lib/python3.8/dist-packages (from tensorboard->simpletransformers) (1.3.0)
Requirement already satisfied: werkzeug>=1.0.1 in /usr/local/lib/python3.8/dist-packages (from tensorboard->simpletransformers) (1.0.1)
Requirement already satisfied: tensorboard-data-server<0.7.0,>=0.6.0 in /usr/local/lib/python3.8/dist-packages (from tensorboard->simpletransformers) (0.6.1)
Requirement already satisfied: google-auth<3,>=1.6.3 in /usr/local/lib/python3.8/dist-packages (from tensorboard->simpletransformers) (2.16.0)
Requirement already satisfied: google-auth-oauthlib<0.5,>=0.4.1 in /usr/local/lib/python3.8/dist-packages (from tensorboard->simpletransformers) (0.4.6)
Requirement already satisfied: tensorboard-plugin-wit>=1.6.0 in /usr/local/lib/python3.8/dist-packages (from tensorboard->simpletransformers) (1.8.1)
Requirement already satisfied: markdown>=2.6.8 in /usr/local/lib/python3.8/dist-packages (from tensorboard->simpletransformers) (3.4.1)
Requirement already satisfied: toolz in /usr/local/lib/python3.8/dist-packages (from altair>=3.2.0->streamlit->simpletransformers) (0.12.0)
Requirement already satisfied: jsonschema>=3.0 in /usr/local/lib/python3.8/dist-packages (from altair>=3.2.0->streamlit->simpletransformers) (4.3.3)
Requirement already satisfied: entrypoints in /usr/local/lib/python3.8/dist-packages (from altair>=3.2.0->streamlit->simpletransformers) (0.4)
Requirement already satisfied: jinja2 in /usr/local/lib/python3.8/dist-packages (from altair>=3.2.0->streamlit->simpletransformers) (2.11.3)
Requirement already satisfied: six>=1.4.0 in /usr/local/lib/python3.8/dist-packages (from docker-pycreds>=0.4.0->wandb>=0.10.32->simpletransformers) (1.15.0)
Requirement already satisfied: multidict<7.0,>=4.5 in /usr/local/lib/python3.8/dist-packages (from aiohttp->datasets->simpletransformers) (6.0.4)
Requirement already satisfied: attrs>=17.3.0 in /usr/local/lib/python3.8/dist-packages (from aiohttp->datasets->simpletransformers) (22.2.0)
Requirement already satisfied: charset-normalizer<3.0,>=2.0 in /usr/local/lib/python3.8/dist-packages (from aiohttp->datasets->simpletransformers) (2.1.1)
Requirement already satisfied: yarl<2.0,>=1.0 in /usr/local/lib/python3.8/dist-packages (from aiohttp->datasets->simpletransformers) (1.8.2)
Requirement already satisfied: aiosignal>=1.1.2 in /usr/local/lib/python3.8/dist-packages (from aiohttp->datasets->simpletransformers) (1.3.1)
Requirement already satisfied: frozenlist>=1.1.1 in /usr/local/lib/python3.8/dist-packages (from aiohttp->datasets->simpletransformers) (1.3.3)
Requirement already satisfied: async-timeout<5.0,>=4.0.0a3 in /usr/local/lib/python3.8/dist-packages (from aiohttp->datasets->simpletransformers) (4.0.2)
Collecting gitdb<5,>=4.0.1
  Downloading gitdb-4.0.10-py3-none-any.whl (62 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 62.7/62.7 KB 7.1 MB/s eta 0:00:00
Requirement already satisfied: pyasn1-modules>=0.2.1 in /usr/local/lib/python3.8/dist-packages (from google-auth<3,>=1.6.3->tensorboard->simpletransformers) (0.2.8)
Requirement already satisfied: rsa<5,>=3.1.4 in /usr/local/lib/python3.8/dist-packages (from google-auth<3,>=1.6.3->tensorboard->simpletransformers) (4.9)
Requirement already satisfied: requests-oauthlib>=0.7.0 in /usr/local/lib/python3.8/dist-packages (from google-auth-oauthlib<0.5,>=0.4.1->tensorboard->simpletransformers) (1.3.1)
Requirement already satisfied: zipp>=0.5 in /usr/local/lib/python3.8/dist-packages (from importlib-metadata>=1.4->streamlit->simpletransformers) (3.11.0)
Requirement already satisfied: pyparsing!=3.0.5,>=2.0.2 in /usr/local/lib/python3.8/dist-packages (from packaging>=20.0->transformers>=4.6.0->simpletransformers) (3.0.9)
Collecting urllib3<1.27,>=1.21.1
  Downloading urllib3-1.26.14-py2.py3-none-any.whl (140 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 140.6/140.6 KB 18.5 MB/s eta 0:00:00
Requirement already satisfied: pygments<3.0.0,>=2.6.0 in /usr/local/lib/python3.8/dist-packages (from rich>=10.11.0->streamlit->simpletransformers) (2.6.1)
Collecting markdown-it-py<3.0.0,>=2.1.0
  Downloading markdown_it_py-2.1.0-py3-none-any.whl (84 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 84.5/84.5 KB 11.5 MB/s eta 0:00:00
Requirement already satisfied: decorator>=3.4.0 in /usr/local/lib/python3.8/dist-packages (from validators>=0.2->streamlit->simpletransformers) (4.4.2)
Collecting smmap<6,>=3.0.1
  Downloading smmap-5.0.0-py3-none-any.whl (24 kB)
Requirement already satisfied: MarkupSafe>=0.23 in /usr/local/lib/python3.8/dist-packages (from jinja2->altair>=3.2.0->streamlit->simpletransformers) (2.0.1)
Requirement already satisfied: pyrsistent!=0.17.0,!=0.17.1,!=0.17.2,>=0.14.0 in /usr/local/lib/python3.8/dist-packages (from jsonschema>=3.0->altair>=3.2.0->streamlit->simpletransformers) (0.19.3)
Requirement already satisfied: importlib-resources>=1.4.0 in /usr/local/lib/python3.8/dist-packages (from jsonschema>=3.0->altair>=3.2.0->streamlit->simpletransformers) (5.10.2)
Collecting mdurl~=0.1
  Downloading mdurl-0.1.2-py3-none-any.whl (10.0 kB)
Requirement already satisfied: pyasn1<0.5.0,>=0.4.6 in /usr/local/lib/python3.8/dist-packages (from pyasn1-modules>=0.2.1->google-auth<3,>=1.6.3->tensorboard->simpletransformers) (0.4.8)
Requirement already satisfied: oauthlib>=3.0.0 in /usr/local/lib/python3.8/dist-packages (from requests-oauthlib>=0.7.0->google-auth-oauthlib<0.5,>=0.4.1->tensorboard->simpletransformers) (3.2.2)
Building wheels for collected packages: seqeval, validators, pathtools
  Building wheel for seqeval (setup.py) ... done
  Created wheel for seqeval: filename=seqeval-1.2.2-py3-none-any.whl size=16179 sha256=a94fbe73f1ce9a40d71741456fb396603e16b171a810c9292e87371338bcaac2
  Stored in directory: /root/.cache/pip/wheels/ad/5c/ba/05fa33fa5855777b7d686e843ec07452f22a66a138e290e732
  Building wheel for validators (setup.py) ... done
  Created wheel for validators: filename=validators-0.20.0-py3-none-any.whl size=19581 sha256=c3706ee049b99e31234a9cdf45700bc89fd4a00c3892bd19bbfc05ee4ce5d8ea
  Stored in directory: /root/.cache/pip/wheels/19/09/72/3eb74d236bb48bd0f3c6c3c83e4e0c5bbfcbcad7c6c3539db8
  Building wheel for pathtools (setup.py) ... done
  Created wheel for pathtools: filename=pathtools-0.1.2-py3-none-any.whl size=8806 sha256=df9ed1ed1bf7c3e839edf1c0294ba68beb600ff880f63de065238b26c59b96c7
  Stored in directory: /root/.cache/pip/wheels/4c/8e/7e/72fbc243e1aeecae64a96875432e70d4e92f3d2d18123be004
Successfully built seqeval validators pathtools
Installing collected packages: tokenizers, sentencepiece, pathtools, xxhash, watchdog, validators, urllib3, smmap, setproctitle, semver, pympler, multiprocess, mdurl, docker-pycreds, blinker, sentry-sdk, pydeck, markdown-it-py, gitdb, seqeval, rich, responses, huggingface-hub, GitPython, wandb, transformers, streamlit, datasets, simpletransformers
  Attempting uninstall: urllib3
    Found existing installation: urllib3 1.24.3
    Uninstalling urllib3-1.24.3:
      Successfully uninstalled urllib3-1.24.3
Successfully installed GitPython-3.1.30 blinker-1.5 datasets-2.8.0 docker-pycreds-0.4.0 gitdb-4.0.10 huggingface-hub-0.11.1 markdown-it-py-2.1.0 mdurl-0.1.2 multiprocess-0.70.14 pathtools-0.1.2 pydeck-0.8.0 pympler-1.0.1 responses-0.18.0 rich-13.2.0 semver-2.13.0 sentencepiece-0.1.97 sentry-sdk-1.13.0 seqeval-1.2.2 setproctitle-1.3.2 simpletransformers-0.63.9 smmap-5.0.0 streamlit-1.17.0 tokenizers-0.13.2 transformers-4.25.1 urllib3-1.26.14 validators-0.20.0 wandb-0.13.9 watchdog-2.2.1 xxhash-3.2.0
[ ]
import json
with open("//content//drive//MyDrive// bert//train1.json") as read_file:
    train = json.load(read_file)
     
[ ]
train
{"\ufeff[{'context':'The total insurance is calculated monthly.',\n  'qas': [{'id': '00001',\n    'is_impossible': False,\n    'question': 'How often total insurance is calculated?',\n    'answers': [{'text':'monthly', 'answer_start': 34}]}]},\n {'context':'later they will pay you half a month in arrears and full month in advance on basis of occupation.',\n  'qas': [{'id': '00002',\n    'is_impossible': False,\n    'question': 'How to pay the total disability?',\n    'answers': [{'text':'half a month in arrears and full month in advance', 'answer_start': 22}]},\n   {'id': '00003',\n    'is_impossible': False,\n    'question': 'What the definition of total insurance depends on?',\n    'answers': [{'text': 'occupation',\n      'answer_start':86}]},\n   {'id': '00004',\n    'is_impossible': True,\n    'question':'The definition of total disability for occupation category as MP, AA, A, B or C?',\n    'answers':[]}]}]": None}
[ ]

[ ]
with open(r"/content/drive/MyDrive/ bert/test1.json", "r") as read_file:
    test = json.load(read_file)
[ ]
test
{"\ufeff[{'context':'The total insurance is calculated monthly.',\n  'qas': [{'id': '00001',\n    'is_impossible': False,\n    'question': 'How often total insurance is calculated?',\n    'answers': [{'text':'monthly', 'answer_start': 34}]}]},\n {'context':'later they will pay you half a month in arrears and full month in advance on basis of occupation.',\n  'qas': [{'id': '00002',\n    'is_impossible': False,\n    'question': 'How to pay the total disability?',\n    'answers': [{'text':'half a month in arrears and full month in advance', 'answer_start': 22}]},\n   {'id': '00003',\n    'is_impossible': False,\n    'question': 'What the definition of total insurance depends on?',\n    'answers': [{'text': 'occupation',\n      'answer_start':86}]},\n   {'id': '00004',\n    'is_impossible': True,\n    'question':'The definition of total disability for occupation category as MP, AA, A, B or C?',\n    'answers':[]}]}]": None}
[ ]

import logging

from simpletransformers.question_answering import QuestionAnsweringModel, QuestionAnsweringArgs
[ ]
model_type="bert"
model_name= "bert-base-cased"
if model_type == "bert":
    model_name = "bert-base-cased"

elif model_type == "roberta":
    model_name = "roberta-base"

elif model_type == "distilbert":
    model_name = "distilbert-base-cased"

elif model_type == "distilroberta":
    model_type = "roberta"
    model_name = "distilroberta-base"

elif model_type == "electra-base":
    model_type = "electra"
    model_name = "google/electra-base-discriminator"

elif model_type == "electra-small":
    model_type = "electra"
    model_name = "google/electra-small-discriminator"

elif model_type == "xlnet":
    model_name = "xlnet-base-cased"
[ ]
# Configure the model 
model_args = QuestionAnsweringArgs()
model_args.train_batch_size = 16
model_args.evaluate_during_training = True
model_args.n_best_size=3
model_args.num_train_epochs=5
[ ]

### Advanced Methodology
train_args = {
    "reprocess_input_data": True,
    "overwrite_output_dir": True,
    "use_cached_eval_features": True,
    "output_dir": f"outputs/{model_type}",
    "best_model_dir": f"outputs/{model_type}/best_model",
    "evaluate_during_training": True,
    "max_seq_length": 128,
    "num_train_epochs": 5,
    "evaluate_during_training_steps": 1000,
    "wandb_project": "Question Answer Application",
    "wandb_kwargs": {"name": model_name},
    "save_model_every_epoch": False,
    "save_eval_checkpoints": False,
    "n_best_size":3,
    # "use_early_stopping": True,
    # "early_stopping_metric": "mcc",
    # "n_gpu": 2,
    # "manual_seed": 4,
    # "use_multiprocessing": False,
    "train_batch_size": 128,
    "eval_batch_size": 64,
    # "config": {
    #     "output_hidden_states": True
    # }
}
[ ]

model = QuestionAnsweringModel(
    model_type,model_name, args=train_args
)

[ ]

### Remove output folder
!rm -rf outputs
[ ]

# Train the model
model.train_model(train, eval_data=test)

[ ]

# Evaluate the model
result, texts = model.eval_model(test)

[ ]

# Make predictions with the model
to_predict = [
    {
        "context": "The total disability benefit is calculated monthly.",
        "qas": [
            {
                "question": "How often total disability is calculated?",
                "id": "1",
            }
        ],
    }
]
[ ]
answers, probabilities = model.predict(to_predict)

print(answers)

[ ]
convert squad examples to features: 100%|██████████| 1/1 [00:00<00:00, 4744.69it/s]

add example index and unique id: 100%|██████████| 1/1 [00:00<00:00, 658.45it/s]
Running Prediction:   0%|          | 0/1 [00:00<?, ?it/s]
[{'id': '1', 'answer': ['monthly']}]
[ ]
# Make predictions with the model
to_predict = [
    {
        "context": "the payment will be half a month in arrears and half a month in advance.",
        "qas": [
            {
                "question": "How to pay the total disability?",
                "id": "2",
            }
        ],
    }
]
[ ]
convert squad examples to features: 100%|██████████| 1/1 [00:00<00:00, 4744.69it/s]

add example index and unique id: 100%|██████████| 1/1 [00:00<00:00, 658.45it/s]
Running Prediction:   0%|          | 0/1 [00:00<?, ?it/s]
[{'id': '2', 'answer': ['half a month in arrears and half a month in advance']}]
[ ]
# Make predictions with the model
to_predict = [
    {
        "context": "The definition of totally disabled depends on the person insured’s occupation category.",
        "qas": [
            {
                "question": "What the definition of total disability depends on?",
                "id": "3",
            }
        ],
    }
]
[ ]
convert squad examples to features: 100%|██████████| 1/1 [00:00<00:00, 4744.69it/s]

add example index and unique id: 100%|██████████| 1/1 [00:00<00:00, 658.45it/s]
Running Prediction:   0%|          | 0/1 [00:00<?, ?it/s]
[{'id': '3', 'answer': ['occupation']}]
[ ]

[ ]

Colab paid products - Cancel contracts here
