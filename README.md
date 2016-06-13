# Fine-Tuned word embeddings trained on the Community Question Answering data of QatarLiving.com forum as used in Semanticz System in the SemEval 2016 Task 3 Community Question Answering
Here we publish our fine-tuned domain specific word embeddings suitable for Community Question Answering in the Qatar Living Forum as used for SemanticZ system participation in Semeval 2016 Task 3 Community Question Answering.

## SemEval 2016 Task 3 Community Question Answering
Official page - [http://alt.qcri.org/semeval2016/task3/](http://alt.qcri.org/semeval2016/task3/)

Description paper and results - [pdf](http://alt.qcri.org/semeval2016/task3/data/uploads/semeval2016-task3-report.pdf)

##SemanticZ at SemEval-2016 Task 3: Ranking Relevant Answers in Community Question Answering Using Semantic Similarity Based on Fine-tuned Word Embeddings
We publish word2vec word embeddings trained on Qatar Living([qatarliving.com](http://qatarliving.com)) questions and answers as used in our system for finding good answers in a community forum, as defined in SemEval-2016, Task 3 on Community Question Answering. Our approach relies on several semantic similarity features based on fine-tuned word embeddings and topics similarities. In the main Subtask C, our primary submission was ranked third, with a MAP of 51.68 and accuracy of 69.94. In Subtask A, our primary submission was also third, with MAP of 77.58 and accuracy of 73.39.

System description paper:[pdf]()
Authors: [Todor Mihaylov](http://www.cl.uni-heidelberg.de/~mihaylov/) and [Preslav Nakov](http://qcri.org.qa/page?a=117&pid=35&lang=en-CA)
##Resources

Please, cite the following paper if you use the resources below:
```bib
@InProceedings{mihaylov-nakov:2016:SemEval,
  author    = {Mihaylov, Todor  and  Nakov, Preslav },
  title     = {SemanticZ at SemEval-2016 Task 3: Ranking Relevant Answers in Community Question Answering Using Semantic Similarity Based on Fine-tuned Word Embeddings},
  booktitle = {Proceedings of the 10th International Workshop on Semantic Evaluation (SemEval 2015)},
  month     = {June},
  year      = {2016},
  address   = {San Diego, California},
  publisher = {Association for Computational Linguistics},
  pages     = {00 - 00},
  url       = {http://www.aclweb.org/anthology/S16}
}
```

**Table:Semantic vectors of different vector sizes + cossim(vec(Q),vec(A)), trained on Qatar Living Forum as features for subtask A:** training on train2016-part1, testing on test2016:

| Vector size | MAP | Accuracy | Word embeddings |
| --- | --- | --- | --- |
| 800 | **78.45** | 74.22 | [Download](https://www.amazon.com/clouddrive/share/1EB78q7aMEALf4x0OCSG9qhJttOCdwts9jJWu173Ilu) | 
| 700 | 78.12 | 73.98 | [Download](https://www.amazon.com/clouddrive/share/aHmE1GukQrOpP6xDbtglo5bmBs3F7EqSSYvVTBMosWr) |
| 600 | 77.31 | 73.15 | [Download](https://www.amazon.com/clouddrive/share/M03CdHKAOLiTFV1Zvgf6HG6dVI4EGGILqLSlOgd8SJK) |
| 500 | 77.61 | 73.30 | [Download](https://www.amazon.com/clouddrive/share/s0R7cokzecUfGy35uPoJO0tMvaiLqwsQ2eN7dU2H3XS) |
| 400 | 78.36 | 74.19 | - |
| 300 | 77.25 | 74.50 | [Download](https://www.amazon.com/clouddrive/share/ifW3RP6ahKmKQkVazv3DlnLLKT06FZLFS2LlAY6WK36) |
| 200 | 77.90 | 73.88 | [Download](https://www.amazon.com/clouddrive/share/7qBwXmkX0zRoAtdnlNE9nqLipqo5AotHdnUHovD5opW) |
| 100 | 77.08 | **74.53** | [Download](https://www.amazon.com/clouddrive/share/kF8IOxppcWusScsfY7lE0R1g0GfU2C7teSKDiDZXGym) |
| 50 | 77.22 | 73.85 | - |
| 20 | 75.44 | 72.42 | [Download](https://www.amazon.com/clouddrive/share/H7YTNXMkNCP0TH5tMWrYIygIBGwCRPPTLeEMS4QaHwX) |
| Baseline | 59.53 | - | 


**Table:Exploring Word2Vec training parameters on Qatar Living Forum:** word vector size (Size), context window (Window), minimum word frequency (Freq), and skip-grams (Skip).
Vectors used as features for subtask A (together with all other features):
training on train2016-part1, testing on test2016:

| Size  |  Window  |  Freq  |  Skip | MAP | Acc | Word embeddings |
| --- | --- | --- |  --- | --- | --- | --- |
| 200 |   5 |   1 |   3  |  **78.21** | 74.25 | [Download](https://www.amazon.com/clouddrive/share/QSa5PwTTPG97rEUdrUfRwDGl1Vj7YhcFUIj2s0j0RY3)  - best performing for Subtask A with ablated features(see table below)|
| 200 |   5 |   5 |   1 | 78.19 | 73.49 | [Download](https://www.amazon.com/clouddrive/share/7gnbjmbf8jsGbz7nLdGA2TRvIpoiQuJAk4yNM6h4xRl) |
| 200 |   5 |   5 |   3 | 78.13 | 74.01 | [Download](https://www.amazon.com/clouddrive/share/QTxFpXYTYqGSEJIYadNXsmb0YcPIRrJakmndkzsemwH) |
| 200 |   5 |   1 |   1 | 78.01  |  74.53 | [Download](https://www.amazon.com/clouddrive/share/7DqnkQ8b2NZovFmuXwX0ylW8iAf4vbGg13nLJlV4b2V) |
| 100 |   5 |   1 |   1 | 77.93 | 74.19 | [Download](https://www.amazon.com/clouddrive/share/oFqMjFXfc0Mt8YvmVDWPIjoLVqQ2vAli9w68Q7f4k6y) - best performing for Subtask C with ablated features(see table below)|
| 200 |   10 |   5 |   1 | 77.90 | 73.88 | [Download](https://www.amazon.com/clouddrive/share/7qBwXmkX0zRoAtdnlNE9nqLipqo5AotHdnUHovD5opW) |
| 100 |   5 |   1 |   3 | 77.81 | 73.94 | [Download](https://www.amazon.com/clouddrive/share/IznHeZ7X42XVNQM6SwSDSK4c9b2rFq8xje2fESFTkt2) |
| 100 |   10 |   1 |   1 | 77.72 | 74.43 | [Download](https://www.amazon.com/clouddrive/share/dCg6GXVlAJN0Dx6soo7Fv3nebV88f1zdNp4k3iXPYHT) |
| 200 |   10 |   1 |   1 | 77.58 | 74.25 | [Download](https://www.amazon.com/clouddrive/share/WAsDY6PqTl0LaOUil3mNWKI4d2IJ109XeIRLQvbTbrw) |
| 100 |   5 |   5 |   1 | 77.53 | 74.07 | [Download](https://www.amazon.com/clouddrive/share/EKebZOiuuJpadx23pEKUqyF0MbEBz1TPhjd65rkQ0VO) |
| 200 |   10 |   1 |   3 | 77.43 | 73.73 | [Download](https://www.amazon.com/clouddrive/share/tS7Q8ab9Bte3vjQRLzH88CNanBA7tlptlo4bywmyKTQ) |
| 100 |   10 |   10 |   1 | 77.18 | 73.79 | - |
| 100 |   10 |   5 |   1 | 77.08  |  **74.53** | [Download](https://www.amazon.com/clouddrive/share/kF8IOxppcWusScsfY7lE0R1g0GfU2C7teSKDiDZXGym) |


**Table: Subtask C. Using all features without some feature groups.** Word2Vec is trained on QL with word vector size 100, context window 5, minimum word frequency 1, and skip-grams 1 ([Download](https://www.amazon.com/clouddrive/share/oFqMjFXfc0Mt8YvmVDWPIjoLVqQ2vAli9w68Q7f4k6y)), Classifier is trained on Train2016-part1 and evaluated on Test-2016:

| Features | MAP | Accuracy |
| --- | --- | --- |
| All  -  Q to C sim              | **53.39** | 69.87 |
| All  -  Meta categories         | 53.06 | 69.81 |
| All  -  WC sim and Meta cat      | 52.91 | 69.54 |
| All  -  WC sim and LDA sim       | 52.84 | 70.06 |
| All  -  Meta cat and LDA sim         | 52.83 | 69.87 |
| All  -  Ext POS sim and WC sim   | 52.82 | 70.21 |
| All                             | 52.78 | 69.43 |
| All  -  Aligned similarity      | 52.76 | 70.10 |
| All  -  Word Clusters similarity | 52.58 | 69.63 |
| All  -  Maximized similarity    | 52.47 | 69.27 |
| All  -  Cat and WC and LDA sim | 52.44 | 69.51 |
| All  -  Ext POS sim             | 52.23 | 69.91 |
| All  -  LDA sim                 | 52.08 | 69.97 |
| All  -  POS sim                 | 51.57 | 69.96 |
| All  -  Word Vectors            | 49.57 | 70.13 |
| All  -  Metadata full           | 46.03 | **71.06** |
| Primary | 51.68 | 69.94 |
| Contrastive 1  | 51.46 | 69.69 |
| Contrastive 2 | 48.76 | 69.71 |
| Baseline (IR) | 28.88 | -- |

**Table:Subtask A. Using all features without some feature groups.**
Word2Vec is trained with word vector size 200, context window 5, minimum word frequency 1, and skip-grams 3([Download](https://www.amazon.com/clouddrive/share/QSa5PwTTPG97rEUdrUfRwDGl1Vj7YhcFUIj2s0j0RY3)). Classifier is trained on Train2016-part1 and evaluated on Test-2016:

| Features | MAP  | Accuracy |
| --- | --- | --- |
| All  -  Quest. to Comment sim | **78.52** | 74.31 |
| All  -  Maximized similarity       | 78.38 | 74.59 |
| All  -  Word Clusters similarity   | 78.29 | 74.25 |
| All  -  WC sim \& Meta cat        | 78.22 | 74.04 |
| All  -  Meta categories            | 78.21 | 74.25 |
| All                                | 78.21 | 74.25 |
| All  -  Meta cat \& LDA sim           | 78.18 | 73.88 |
| All  -  Ext POS sim \& WC sim     | 78.10 | 74.28 |
| All  -  Aligned similarity         | 77.97 | 74.16 |
| All  -  Cat \& WC \& LDA sim | 77.95 | 74.19 |
| All  -  WC \& LDA sims         | 77.92 | 74.25 |
| All  -  Ext POS sim                | 77.92 | 74.43 |
| All  -  LDA sim                    | 77.85 | 74.37 |
| All  -  POS sim                    | 77.77 | **74.80** |
| All  -  Metadata full              | 74.50 | 70.31 |
| All  -  Word Vectors               | 74.35 | 70.80 |
| Primary                            | 77.58 | 73.39 |
| Contrastive 1                      | 77.16 | 73.88 |
| Contrastive 2                      | 75.41 | 72.26 |
| Baseline (IR)  | 59.53 | --  |


##How to use the embeddings
The emebeddings published here can be used using [gensim](https://radimrehurek.com/gensim/models/word2vec.html) word2vec implementation.

```python
word2vec_model_file='qatarliving_qc_size200_win5_mincnt1_rpl_skip3_phrFalse_2016_02_25.word2vec.bin' # put here the .bin file from the downloaded zip file

#load the model
model = Word2Vec.load_word2vec_format(word2vec_model_file, binary=False) # binary should be False

#evaluate
model.most_similar(positive=['woman', 'king'], negative=['man'], topn=1)

#get embedding for word
model['qatar']

```
For more examples of using the loaded model, please see the Gensim Word2Vec tutorial by Radim Rehurek [here](http://rare-technologies.com/word2vec-tutorial/).

##Questions and issues with the embeddings
If you have any questions or problems with the embeddings, please open an issue or send an e-mail to tbmihailov [at] gmail!
