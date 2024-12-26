# MLOPS-COMPLETED-ML-PIPELINE
HOW TO AUTOMATE PIPELINE WITH DVC

Building Pipeline:
1> Create a GitHub repo and clone it in local (Add experiments).
2> Add src folder along with all components(run them individually).
3> Add data, models, reports directories to .gitignore file
4> Now git add, commit, push

Setting up dcv pipeline (without params)
5> Create dvc.yaml file and add stages to it.
6> dvc init then do "dvc repro" to test the pipeline automation. (check dvc dag)
7> Now git add, commit, push

Setting up dcv pipeline (with params)
8> add params.yaml file
9> Add the params setup (mentioned below)
10> Do "dvc repro" again to test the pipeline along with the params
11> Now git add, commit, push

Expermients with DVC:
12> pip install dvclive
13> Add the dvclive code block (mentioned below)
14> Do "dvc exp run", it will create a new dvc.yaml(if already not there) and dvclive directory (each run will be considered as an experiment by DVC)
15> Do "dvc exp show" on terminal to see the experiments or use extension on VSCode (install dvc extension)
16> Do "dvc exp remove {exp-name}" to remove exp (optional) | "dvc exp apply {exp-name}" to reproduce prev exp
17> Change params, re-run code (produce new experiments)
18> Now git add, commit, push
