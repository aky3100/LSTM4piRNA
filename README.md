# LSTM4piRNA
Efficient computational detection of piRNAs using LSTM Network. This repository contains the source code for LSTM4piRNA from the paper "LSTM4piRNA: Efficient piRNA Detection in Large-Scale Genome Databases using a Deep Learning-Based LSTM Network." Please cite the paper if you use our source code or data.

## Usage
The users are welcome to use LSTM4piRNA webserver available at https://redfold.ee.ncyu.edu.tw for RNA structure prediction.
REDfold is implemented in Python code and the cross-platform compatible program can be installed through the [wheel package](https://lstm4pirna.ee.ncyu.edu.tw).
It can predict the RNA secondary structure based on the RNA sequences.

### System Requirement
 python (>=3.7)  
 biopython (>=1.79)  
 numpy (>=1.21)  
 pandas(>=1.3.5)  
 scipy (>=1.7.3)  
 torch (>=1.9+cu111) 

### Installation
REDfold can be installed through the [wheel package](https://redfold.ee.ncyu.edu.tw).
```
% pip install redfold-1.14a0-py2.py3-none-any.whl
```

### Test data
LSTM4piRNA can predict the RNA secondary structure with fasta-formatted RNA sequences.
```
% lstm4pirna directory_containing_fasta_files
>D00002586
GCUCGCGUGGCGUAAUGGCAACGCGUCUGACUUCUAAUCAGAAGAUUAUGGGUUCGACCCCCAUCGUGAGUG

```


### Train model
LSTM4piRNA can train the parameters with BPSEQ-formatted RNA sequences.
```
% lstm4pirna -train directory_negative_files directory_positive_files
```

## Web Server
LSTM4piRNA web server is available at https://lstm4pirna.ee.ncyu.edu.tw

## Reference
Chun-Chi Chen, Yi-Ming Chan, and Hyundoo Jeong, ""LSTM4piRNA: Efficient piRNA Detection in Large-Scale Genome Databases using a Deep Learning-Based LSTM Network."
