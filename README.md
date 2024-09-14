# llmexpress
Run LLM models locally with a single script




Almost every week a new model is being released and they are really work of art. But you might have a very specific use case and you want to run the model locally and test it out. So, this process of testing a model should be fast and easy enough to do.

There are good tools available for similar purposes like [Hugging Face Transformers](https://huggingface.co/transformers/) and or [Ollama](https://ollama.com/) later being the easiest to use. But what if we wanted to keep the dependencies to minimum and wanted to run the model locally. And can be used by the non technical users as well. This is where LLMExpress comes in.


Idea is simple, one script which takes a model link, a prompt and runs the model locally. Does all the setup required to run the model and then runs the model. And should be customizable enough to add more features as required.


I am using [llama.cpp](https://github.com/ggerganov/llama.cpp) for inference as it is one of the fastest inference engines available. It is Open source and comes with great documentation. 


## Here's how it works
1. You get the model link from hugging face.
2. You run the script with the model link and the prompt.
3. The script will download the model and the tokenizer.
4. It will then run the model with the prompt.
5. The output will be displayed on the screen.
6. You can keep the conversation going by providing more prompts.
7. Now as you keep downloading more models, tokenizer downloads will be skipped if they are already downloaded. And you will be presented with a li st of models to choose from. So your own local model hub.
