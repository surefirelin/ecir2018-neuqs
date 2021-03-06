# Generating High-Quality Query Suggestion Candidates for Task-Based Search

This repository provides resources developed within the following paper:

> H. Ding, S. Zhang, D. Garigliotti, and K. Balog. **Generating High-Quality Query Suggestion Candidates for Task-Based Search.** In: Advances in Information Retrieval - Proceedings of the 40th European Conference on IR Research (ECIR'18). Springer. Grenoble, France. March 2018. [DOI: 10.1007/978-3-319-76941-7_54](https://link.springer.com/chapter/10.1007/978-3-319-76941-7_54)

**You can get the author version of the article [here](https://arxiv.org/abs/1802.07997).**

### Abstract

> *We address the task of generating query suggestions for task-based search. The current state of the art relies heavily on suggestions provided by a major search engine. In this paper, we solve the task without reliance on search engines. Specifically, we focus on the first step of a two-stage pipeline approach, which is dedicated to the generation of query suggestion candidates. We present three methods for generating candidate suggestions and apply them on multiple information sources. Using a purpose-built test collection, we find that these methods are able to generate high-quality suggestion candidates.* 


### Structure

This repository is structured as follows:

 - `data/`: TSV file used for evaluating the query suggestions. It was obtained by post-processing the test collection (details in the paper).

 - `output/`: all the final TSV run files, containing query suggestions generated by different methods and sources used in the paper.


## Results

Results presented in the paper can be obtained by running the evaluation script, indicating the metrics of interest.

```
$ python eval.py 10  # P@10
$ python eval.py 20  # P@20
```

## Crowdsourcing experiments

We seek to measure the quality of question suggestions for task-based search. Please see details below.

![Experiment Layout](https://github.com/iai-group/ecir2018-neuqs/blob/master/images/exp_layout.png)


## Citation

If you use the resources presented in this repository, please cite:

```
@InProceedings{Ding:2018:GHQ,
 author =     {Ding, Heng
   and Zhang, Shuo
   and Garigliotti, Dar{\'i}o
   and Balog, Krisztian},
 title =      {Generating High-Quality Query Suggestion Candidates for Task-Based Search},
 booktitle =  {Advances in Information Retrieval - Proceedings of the 40th European Conference on IR Research},
 series =     {ECIR '18},
 year =       {2018},
 pages =      {625--631},
 publisher =  {Springer},
 doi =        {10.1007/978-3-319-76941-7_54},
}
```


## Contact

Should you have any questions, please contact Darío Garigliotti at dario.garigliotti[AT]uis.no (with [AT] replaced by @).
