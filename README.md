# sbert-spanish

Notebooks to train and evaluate sentence transformers models (using Spanish datasets)

# Base model

The trained models are fine-tuned versions of [PlanTL-GOB-ES/roberta-base-bne](https://huggingface.co/PlanTL-GOB-ES/roberta-base-bne) focused on question/answer using two versions of the MS-MARCO dataset translated into Spanish.

# Datasets

* https://huggingface.co/datasets/dariolopez/ms-marco-es (query - positive - negative)
* https://huggingface.co/datasets/IIC/ms_marco_es (query - passage - label)

# Models trained

We have trained several versions, using different configurations:

1. Model 1
  * Dataset: dariolopez/ms-marco-es;
  * Loss: TripletLoss
  * [Link](https://huggingface.co/dariolopez/roberta-base-bne-finetuned-msmarco-qa-es)
  * [Config](https://huggingface.co/dariolopez/roberta-base-bne-finetuned-msmarco-qa-es/blob/main/train_config.json)

1. Model 2
  * Dataset: dariolopez/ms-marco-es;
  * Loss: MultipleNegativesRankingLoss
  * Link (in progress)
  * Config (in progress)

1. Model 3
  * Dataset: IIC/ms_marco_es;
  * Loss: MultipleNegativesRankingLoss
  * Link (in progress)
  * Config (in progress)

# Resources

* https://www.sbert.net/index.html
* https://github.com/UKPLab/sentence-transformers 
* https://www.pinecone.io/learn/nlp/ 
