# LSTM4piRNA
Efficient computational detection of piRNAs using LSTM Network. This repository contains the source code for LSTM4piRNA from the paper "LSTM4piRNA: Efficient piRNA Detection in Large-Scale Genome Databases using a Deep Learning-Based LSTM Network." Please cite the paper if you use our source code or data.

## Usage
The users are welcome to use LSTM4piRNA webserver available at https://lstm4pirna.ee.ncyu.edu.tw for RNA prediction.
LSTM4piRNA is implemented in Python code and the cross-platform compatible program can be installed through the [wheel package](https://lstm4pirna.ee.ncyu.edu.tw).
It can predict the piRNA based on the RNA sequences.

### System Requirement
 python (>=3.7)  
 biopython (>=1.79)  
 numpy (>=1.21)  
 pandas(>=1.3.5)  
 scipy (>=1.7.3)  
 torch (>=1.9+cu111) 

### Installation
LSTM4piRNA can be installed through the [wheel package](https://lstm4pirna.ee.ncyu.edu.tw).
```
% pip install lstm4pirna-1.11a0-py2.py3.whl
```

### Test data
LSTM4piRNA can predict the RNA secondary structure with fasta-formatted RNA sequences.
```
% lstm4pirna directory_containing_fasta_files
>PiRNA_Human 1.00001
UGGAGAUGAAGUGCAAAGAAAUAAAGUGA

```


### Train model
LSTM4piRNA can train the parameters with BPSEQ-formatted RNA sequences.
```
% lstm4pirna -train directory_positive_files directory_negative_files
```

## Web Server
LSTM4piRNA web server is available at https://lstm4pirna.ee.ncyu.edu.tw

## Reference
Chun-Chi Chen, Yi-Ming Chan, and Hyundoo Jeong, "LSTM4piRNA: Efficient piRNA Detection in Large-Scale Genome Databases using a Deep Learning-Based LSTM Network." IJMS (2023).
