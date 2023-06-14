# sbert-spanish

Notebooks to train and evaluate sentence transformers models (using Spanish datasets)

# Base model

The trained models are fine-tuned versions of [PlanTL-GOB-ES/roberta-base-bne](https://huggingface.co/PlanTL-GOB-ES/roberta-base-bne) focused on question/answer using two versions of the MS-MARCO dataset translated into Spanish.

# Models trained

We have trained several versions, using different configurations:

* **Model 1**
  * [Link](https://huggingface.co/dariolopez/roberta-base-bne-finetuned-msmarco-qa-es)
  * [Config](https://huggingface.co/dariolopez/roberta-base-bne-finetuned-msmarco-qa-es/blob/main/train_config.json)
  * Dataset: [dariolopez/ms-marco-es](https://huggingface.co/datasets/dariolopez/ms-marco-es) (query - positive - negative)
  * Loss: TripletLoss

* **Model 2**
  * [Link](https://huggingface.co/dariolopez/roberta-base-bne-finetuned-msmarco-qa-es-mnrl-mn)
  * [Config](https://huggingface.co/dariolopez/roberta-base-bne-finetuned-msmarco-qa-es-mnrl-mn/blob/main/train_config.json)
  * Dataset: [IIC/ms_marco_es](https://huggingface.co/datasets/IIC/ms_marco_es) (query - positive - negative - negative - negative - negative)
  * Loss: MultipleNegativesRankingLoss

* **Model 3**
  * Link (in progress)
  * Config (in progress)
  * Dataset: [dariolopez/ms-marco-es](https://huggingface.co/datasets/dariolopez/ms-marco-es) (query - positive - negative)
  * Loss: MultipleNegativesRankingLoss

# Resources

* https://www.sbert.net/index.html
* https://github.com/UKPLab/sentence-transformers 
* https://www.pinecone.io/learn/nlp/ 
