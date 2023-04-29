# Big_data_project1
## Preprocess.ipynb
### This file is responsible for data preprocessing and it achieves following tasks:
1. Cut reads and reference bins into kmers. There are two kmer size, 15 and 20.
2. Create two ditsinct kmer lists based on all kmers from reads and reference bins. The number of disticnt kmer with kmer size = 15 is 
72530 and the number of distinct kmer with kmer size = 20 is 77751
3. Use previously created kmer lists to encode read and reference bins. For kmer size as 15, shape of reads' one-hot encoding result is 72530 * 2000; shape of reference bins' one-hot encoding result is 72530 * 500. For kmer size as 20, shape of reads' one-hot encoding result is 77751 * 2000; shape of reference bins' one-hot encoding result is 77751 * 500.
4. One-hot encoding results are sparse matrix. Thus, use sparse vectors to store the results for storage save.
5. Store the one-hot encoding results in sparse vector format

## One_hot_encoding_SparseV
This directory contains four files. They are one-hot encoding results in sparse vector format from *Preprocess.ipynb*, respectively read_sparse_15, ref_sparse_15, read_sparse_20, ref_sparse_20. These four files is the input of *Minhash_Comparison_Result.ipynb*

## Minhash_Comparison_Result.ipynb
### This file achieves following tasks:
1. 
