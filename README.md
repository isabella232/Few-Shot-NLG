# Few-shot table-to-text Generation
Generate descriptions from wiki infobox under few shot setting

## Requirements
python3
tensorflow 1.12

## Instructions
Download the data(few_shot_gpt-2.zip) and pre-trained GPT2 model(models.zip), unzip them to the same directory of the code(so that all three of them(few_shot_gpt-2_data, models, wikitobio) are in the same directory).

The training takes two 10G GPUs. I placed the GPT part into one GPU and the pointer generator part into another. 

Command for training:
$ cd wikitobio
$ python Main.py your_saved_model_name

Now it's the experiment on humans domain with 1000 training data. You will see a result bleu score of around 26 after 10 training rounds. 
