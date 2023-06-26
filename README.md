## Project description
jcci is a pure python library that analyzes the impact of two git submissions of Java projects on the project and generates tree chart data
for example:

### Installing jcci
```
  $pip install jcci
```

### Quick start
```
>>> from jcci import jcci
>>> jcci.analyze('git@xxxx.git','master','commit_id1','commit_id2', 'username1')
```
At the same time, the project will be cloned in the directory and then analyzed to generate a file with the suffix format commit_id1...commit_id2.cci, which contains the tree diagram data generated by the analysis results, through https://echarts.apache.org/examples/zh/editor.html?c=tree-basic link, replace the data data can be displayed through the view.

#### CCI result
![result](https://raw.githubusercontent.com/baikaishuipp/jcci/main/cci-result.png)

#### CCI result tree view
![treeView](https://raw.githubusercontent.com/baikaishuipp/jcci/main/cii-result-tree.png)

