### Installation
```bash
# Download the code
git clone https://github.com/PGSmall/DAVIS-Evaluation.git && cd davis2017-evaluation
# Install it - Python 3.6 or higher required
python setup.py install
```
If you don't want to specify the DAVIS path every time, you can modify the default value in the variable `default_davis_path` in `evaluation_method.py`(the following examples assume that you have set it). 
Otherwise, you can specify the path in every call using using the flag `--davis_path /path/to/DAVIS` when calling `evaluation_method.py`.


# DAVIS-Evaluation
I modified the source code [DAVIS2017-Evaluation](https://github.com/davisvideochallenge/davis2017-evaluation), and the revised code can evaluate the davis 2016, 2017 and 2019 datasets.

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

Thanks a lot [issues](https://github.com/davisvideochallenge/davis2017-evaluation/issues/4).
