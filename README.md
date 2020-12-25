# DAVIS-Evaluation
I modified the source code[https://github.com/davisvideochallenge/davis2017-evaluation], and the revised code can evaluate the davis 2016, 2017 and 2019 datasets.

## Evaluate DAVIS 2017 Semi-supervised
In order to evaluate your semi-supervised method in DAVIS 2017, execute the following command substituting `results/semi-supervised/osvos` by the folder path that contains your results:
```bash
python evaluation_method.py --task semi-supervised --results_path results/semi-supervised/osvos --year 2017
```
The semi-supervised results have been generated using [OSVOS](https://github.com/kmaninis/OSVOS-caffe).

## Evaluate DAVIS 2017 Unsupervised
In order to evaluate your unsupervised method in DAVIS 2017, execute the following command substituting `results/unsupervised/rvos` by the folder path that contains your results:
```bash
python evaluation_method.py --task unsupervised --results_path results/unsupervised/rvos --2017
```
The unsupervised results example have been generated using [RVOS](https://github.com/imatge-upc/rvos).

## Evaluate DAVIS 2016 Unsupervised
In order to evaluate your unsupervised method in DAVIS 2017, execute the following command substituting `results/unsupervised/rvos` by the folder path that contains your results:
```bash
python evaluation_method.py --task unsupervised --results_path results/unsupervised/rvos --2016
```
The unsupervised results example have been generated using [RVOS](https://github.com/imatge-upc/rvos).
