# gemma3 1b trainig code for google colab
MAKE SURE YOU HAVE A DATESET THAT ENDS WITH .jsonl FOR GEMMA TO TRAIN ON (recommend using ai to generate)
google colab code for training gemma 3
1.Download the ipynb file for your specific Gemma 3 model
2. sign up to https://www.huggingface.co
3. go to this link to access gemma3 all models (do not mind about the model getting access to one means access to all gemma model) https://huggingface.co/google/gemma-3-4b-it
4. click on your huggingface profile logo and scroll down to access keys
5. click create new key
6. name it colab_gemma
7. copy it as you won't see it again
8. go to http://colab.research.google.com
9. click on file
10. click upload notebook
11. put the specific .ipynb file for a specific gemma model downloaded from this repo in there
12. on the left go to secrets and add a secret and call it HF_TOKEN and paste your huggingface access key in value
13. on the top right click the arrow next to runtime and click change runtime
14. select T4 GPU
15. rename your dataset for the ai to train on file to dataset.jsonl
16. click the folder icon on the left and upload your dataset.jsonl
17. at the top click run all
It will save an ollama model as a .gguf at the end in your google drive
