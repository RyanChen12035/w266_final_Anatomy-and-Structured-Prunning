# Anatomy and Structured Pruning of Large Language Models



Abstract

Large language models have recently achieved state-of-the-art performance across a wide variety of natural language tasks. Meanwhile, as the task of language models gets more complicated, the size of the models also grows drastically so that they become a black box and hard to deploy on edge devices. The mechanism of the Transformer has been fully addressed recently, but as the model gets complicated, the information delivery throughout layers of transformers remains unknown. In this paper, we will parse through both encoder-based BERT and decoder-based GPT2 having twelve layers of the Transformer stacked as the main body of the model, and demonstrate the information delivery of each layer of transformation and neurons in the feed-forward network (FFN) by comparing with the token fed to the classification layer to make the final decision.  In the second part of this paper, we will develop a structured pruning strategy based on the information delivery of the models we got and further prune off the neurons in the feed-forward network (FFN) to solve the issue of latency and still maintain the capability of the models. Current compressing method like network pruning, knowledge distillation, low-rank approximation, and quantization inevitably requires post-training after actions to regain the performance of the model and this takes tons of computational power and time. Here, we will introduce a structured pruning strategy without any costly post-training step while it’s also compatible with every method mentioned


##### BERT_anatomy.ipynb is for figuring out the similarity of layer of Transformers and neuron with cls token of the BERT model
##### GPT2_anatomy.ipynb is for figuring out the similarity of layer of Transformers and neuron with logit token of the GPT2 model
##### BERT_pruning_baseline.ipynb is for arbitarily pruning for the BERT model
##### GPT2_pruning_baseline.ipynb is for arbitarily pruning for the GPT2 model
##### BERT_pruning_strategy.ipynb is for pruning with strategy based on the findings in anatomy
##### GPT2_pruning_strategy.ipynb is for pruning with strategy based on the findings in anatomy

