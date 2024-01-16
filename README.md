# musicgen-finetune
Training pipeline for musicgen using a simple dataset format.

## How to use:
- Follow instructions in the notebook to load dependencies, assuming you have an environment with Jupyter set up.
- Requires access to a GPU with 8+ GB VRAM for training (preferably > 16 GB), at least 4 GB VRAM for inference.
- In Google Colab: replace `input_folder_name` to a path as per your mounted Google Drive (e.g. `/content/...`)

## NOTE:
- Longer outputs take progressively more time in inference, especially depending on your hardware.
- The current model is prone to have silent sections in the ouput, highly influenced by the finetune dataset used (e.g. you use starts and ends of songs).

## TODO
- Support stereo finetune.
- Optimized training: e.g. LORA

## Credits
- Inspired from [a notebook from dominiqueGrys](https://github.com/dominiqueGrys/train-musicGen/blob/main/train_musicGen.ipynb).
- Trainer code from a deleted profile/repository.
- Facebook/Meta research for providing the [tooling](https://facebookresearch.github.io/audiocraft/docs/MUSICGEN.html) to play with their models.
