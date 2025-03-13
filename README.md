# Truncated_SVD_from_Scratch
This repository explains truncated SVD and its code implementaion from scratch. I made this repo with the help from Youtube's video on SVD: Optimal Truncation [Python] by 
Steve Brunton.


## So what is Truncated SVD? 
Before diving into it we first need to understand what is SVD.
SVD stands for Singular Value Decomposition (SVD) is a way to break down a matrix (a table of numbers) into three smaller, simpler matrices, revealing hidden patterns and relationships within the data.
  * It is similar to Principal Component Analysis (PCA), while PCA is used for squre matrices i.e nXn whereas SVD can be used for matrices other than sqaure like nXm where n!=m.

So, SVD is a matrix factorization technique that decomposes any matrix (even non-square ones) into three matrices: U, Σ (Sigma), and Vᵀ (V transpose). 
* U: An orthogonal matrix representing the "left singular vectors". 
* Σ: A diagonal matrix containing the "singular values". 
* Vᵀ: The transpose of an orthogonal matrix representing the "right singular vectors

  ![image](https://github.com/user-attachments/assets/916883bd-7a38-4e8a-a744-096d3b351fd4)


## Now, we get to Truncated SVD.

In simple terms, truncated SVD is a method for reducing the complexity of data (dimensionality reduction) by keeping only the most important parts (singular vectors) while discarding less significant ones. 
* Imagine you have a big table of data (a matrix). SVD is a technique that breaks down this table into smaller, simpler tables that reveal underlying patterns and relationships.
* Instead of keeping all the smaller tables, truncated SVD focuses on the most important ones, effectively reducing the overall size and complexity of the data while preserving the essential information. 


![image](https://github.com/user-attachments/assets/0fcc4f57-f18f-4c32-b9a0-0dc3a2e71f22)

## How it is different in formula:


![image](https://github.com/user-attachments/assets/ea594375-9a4e-48a7-bfa6-49459944c8ca)


## In this repository
I am using **Galvish-Donoho's** method to find these **"k" dimensions** which makes SVD -> Truncated SVD. The formula is explained the notebook so go check it out!!!
