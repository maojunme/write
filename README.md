
## 1. File Folder Structure
The location of the Self-Tunning XGBoosting as an example in Jun’s computer follows a file structure like this:
.* /atlantis/data_analysis/classification/XGB.py

From folder data_analysis onwards each folder contains a __init__.py so that in python, when you set cd to Data_Work_Jun you can call each py script as a function such as:
	cd /home/dataprophet01/Desktop/Data_Work_Jun/
	import data_analysis as da
	da.classification.XGB.atlantis_XGB(x_train, y_train, x_test, y_test, x_new, y_new)

Component of __init__.py in the folder of data_analysis

```python
from . import data_process
from . import classification
from . import data_exploration
from . import multivac
from . import plots
```
This enable you to call data_process, classification, data_exploration etc.. inside data_analysis by python such as da.data_process, da.classification etc..
