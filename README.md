# word-segmentation

## Usage
1. Make sure you have installed [neural transducer](https://github.com/slvnwhrl/il-reimplementation).
2. Download the models for the languages you need from this repository as well as the `predict.py` script.
3. Run `predict.py`:
```
# output folder must exist ("." for current folder)
python predict.py --model-folder model --output PATH_TO_OUTPUT_DIR --test PATH_TO_FILE
```

### Segmentation token
Note that we used a different SINGLE segmentation token to decrease the complexity (as opposed to *@@* in the orginial
shared task data), so check if this token is contained in your test data (if so, change it manually in the loaded vocabulary instance).
