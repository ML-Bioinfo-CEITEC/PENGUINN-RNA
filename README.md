# Penguinn-RNA

PENGUINN-RNA is a machine learning method based on Convolutional Neural Networks, that learns the characteristics of RNA G4 sequences and predicts the probability that a given sequence can form G4.


### Prerequisities

Penguinn is implemented in python using Keras and Tensorflow backend.

Required:

* python, recommended version 3.7
    * Keras 2.3.1
    * tensorflow 2.3.0
    * Biopython
    * numpy

### Installing
First, create a virtual environment.
```
python -m venv venv
```
Then, activate it and install the necessary libraries.
```
source venv/bin/activate
pip install -r requirements.txt
```

### Running prediction

Follow the instructions:

```
cd path/to/Penguinn-RNA/directory
#add rights to execute
chmod +x penguinn-rna.py
#if you've followed the installation steps above and aren't actively sourcing from the previously created virtualenv
source venv/bin/activate
#run the prediction
./penguinn-rna.py --input <input_fasta_file> --output <output_file> --model <path_to_model.h5>
```

Default model is set to model trained on human rG4 dataset with positive:negative samples ratio 1:1, as described in our paper.

### Web application

https://ml-bioinfo-ceitec.github.io/PENGUINN-RNA/

### Contact information

CEITEC MU, RBP Bioinformatics - Panagiotis Alexiou, https://www.ceitec.eu/rbp-bioinformatics-panagiotis-alexiou/rg281
