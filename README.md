# [LLM ZoomCamp](https://github.com/DataTalksClub/llm-zoomcamp/)

# LLM-ZoomCamp-Intro

Following this ZoomCamp [workshop](https://www.youtube.com/watch?v=q-p36Ak6YI8&list=PL3MmuxUbc_hKiIVNf7DeEt_tGjypOYtKV&index=2)
More info and step by step guide in [this repo](https://github.com/alexeygrigorev/llm-rag-workshop)
Instead of using codespaces I developed this locally with some small changes to the tooling (like using poetry to manage my dependecies and adding linting and isort to pre-commit etc to follow some best practices)

Design sketch:
![alt text](media/image.png)

Check this for real world implementation: https://github.com/aaalexlit/faq-slack-bot

# To Do

[ ] Cache the responses

---

# Adding semantic search

Source: https://github.com/DataTalksClub/llm-zoomcamp/tree/main/03-vector-search

![alt text](media/image-1.png)

- install [sentence_transformers](https://sbert.net/). With this we can call [pre-trained models available](https://sbert.net/docs/sentence_transformer/pretrained_models.html) and create embeddings
- choose what fields you want to encode - in the case of our documents it would make sense to encode the 'text' field
