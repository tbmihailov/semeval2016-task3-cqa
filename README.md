# Resources used in Semanticz System in the SemEval 2016 Task 3 Community Question Answering
Resources for the Semeval 2016 Task 3 Community Question Answering. Contains word embeddings and system description results
## SemEval 2016 Task 3 Community Question Answering
##SemanticZ at SemEval-2016 Task 3: Ranking Relevant Answers in Community Question Answering Using Semantic Similarity Based on Fine-tuned Word Embeddings
We publish word2vec word embeddings trained on Qatar Living([qatarliving.com](http://qatarliving.com) questions and answers as used in our system for finding good answers in a community forum, as defined in SemEval-2016, Task 3 on Community Question Answering. Our approach relies on several semantic similarity features based on fine-tuned word embeddings and topics similarities. In the main Subtask C, our primary submission was ranked third, with a MAP of 51.68 and accuracy of 69.94. In Subtask A, our primary submission was also third, with MAP of 77.58 and accuracy of 73.39.

System description paper:[pdf]()

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

| Vector size | MAP | Accuracy | - |
| --- | --- | --- | --- |
| 800 | **78.45** | 74.22 | [Download]() | 
| 700 | 78.12 | 73.98 | [Download]() |
| 600 | 77.31 | 73.15 | [Download]() |
| 500 | 77.61 | 73.30 | [Download]() |
| 400 | 78.36 | 74.19 | [Download]() |
| 300 | 77.25 | 74.50 | [Download]() |
| 200 | 77.90 | 73.88 | [Download]() |
| 100 | 77.08 | **74.53** | [Download]() |
| 50 | 77.22 | 73.85 | [Download]() |
| 20 | 75.44 | 72.42 | [Download]() |
| Baseline | 59.53 | - | 


*Table:Exploring Word2Vec training parameters on Qatar Living Forum:* word vector size (Size), context window (Window), minimum word frequency (Freq), and skip-grams (Skip).
Vectors used as features for subtask A (together with all other features):
training on train2016-part1, testing on test2016:

| Size  |  Window  |  Freq  |  Skip | MAP | Acc | - |
| --- | --- | --- |  --- | --- | --- |
| 200 |   5 |   1 |   3  |  **78.21** | 74.25 | [Download]() |
| 200 |   5 |   5 |   1 | 78.19 | 73.49 | [Download]() |
| 200 |   5 |   5 |   3 | 78.13 | 74.01 | [Download]() |
| 200 |   5 |   1 |   1 | 78.01  |  74.53 | [Download]() |
| 100 |   5 |   1 |   1 | 77.93 | 74.19 | [Download]() |
| 200 |   10 |   5 |   1 | 77.90 | 73.88 | [Download]() |
| 100 |   5 |   1 |   3 | 77.81 | 73.94 | [Download]() |
| 100 |   10 |   1 |   1 | 77.72 | 74.43 | [Download]() |
| 200 |   10 |   1 |   1 | 77.58 | 74.25 | [Download]() |
| 100 |   5 |   5 |   1 | 77.53 | 74.07 | [Download]() |
| 200 |   10 |   1 |   3 | 77.43 | 73.73 | [Download]() |
| 100 |   10 |   10 |   1 | 77.18 | 73.79 | [Download]() |
| 100 |   10 |   5 |   1 | 77.08  |  **74.53** | [Download]() |



