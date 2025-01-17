# Enhancing Visual Realism: Fine-Tuning InstructPix2Pix for Advanced Image Colorization (Deeplearning 282A/182)
![image](https://github.com/AllenAnZifeng/DeepLearning282/blob/main/stages.png)
## quickstart
The results below were obtained using a GPU 3080TI.
### WINDOWS
login into huggingface
```
> huggingface-cli login    
```
Confirm that you successfully logged in to huggingface
```
> huggingface-cli whoami 
```
In finetune_instruct_pix2pix.py 

```
parser.add_argument(
        "--hub_token",
        type=str,
        default=None,
        help="The token to use to push to the Model Hub.",
    )
```
replace the `default` from `None` to your huggingface access token.

run the program
```
> ./run_finetune.bat   
```
in run_finetune.bat change "OUTPUT_DIR" into your path.
### LINUX
login into huggingface
```
> huggingface-cli login    
```
Confirm that you successfully logged in to huggingface
```
> huggingface-cli whoami 
```

In finetune_instruct_pix2pix.py 

```
parser.add_argument(
        "--hub_token",
        type=str,
        default=None,
        help="The token to use to push to the Model Hub.",
    )
```
replace the `default` from `None` to your huggingface access token.

run the program
```
> ./run_finetune.sh
```
in run_finetune.sh change "OUTPUT_DIR" into your path.

## Building your own datasets or finetuning work

Make sure you have already logged in huggingface before you start running generate_dataset.py and export_to_hub.py.

By running generate_dataset.py and export_to_hub.py can help you generate your own dataset.
