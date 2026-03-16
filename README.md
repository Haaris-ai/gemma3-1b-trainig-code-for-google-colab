# gemma3 1b trainig code for google colab
google colab code for training gemma 3
1. sign up to https://www.huggingface.co
2. go to this link to access gemma3 all models (do not mind about the model getting access to one means access to all gemma model) https://huggingface.co/google/gemma-3-4b-it
3. click on your huggingface profile logo and scroll down to access keys
4. click create new key
5. name it colab_gemma
6. copy it as you won't see it again
7. go to http://colab.research.google.com
8. click on file
9. click upload notebook
10. put the specific .ipynb file for a specific gemma model downloaded from this repo in there
11. on the left go to secrets and add a secret called HF_TOKEN and paste your huggingface access key in value
12. on the top right click the arrow next to runtime and click change runtime
13. select T4 GPU
14. rename your dataset file to dataset.jsonl
15. click the folder icon on the left and upload your dataset.jsonl
16. at the top click run all
It will save an ollama model as a .gguf at the end in your google drive
