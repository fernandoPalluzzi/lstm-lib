# lstm-lib

The **lstm-lib** library is a simple [**Keras**](https://keras.io/) library for time series prediction using long short-term memory (LSTM) recurrent neural networks. It requires the installation of Python (>= 3.8) and the tensorflow-gpu library (>= 2.4), together with core computational Python libraries, including numpy, pandas, tabulate, scipy, and matplotlib. To facilitate the correct execution of the software, the installation of Conda is recommended (https://docs.conda.io/projects/conda/en/latest/user-guide/install). The lstmContacts repository provides a **tfenv.yml** file that can be used to install all the required dependencies. Please, follow these instructions from a bash terminal:

```
# After installing Conda, activate the base Conda environment.
# If it is already activated, a "(base)" mark will be present before the command line prompt
conda activate

# Install the TensorFlow environment
conda env create -f tfenv.yml

# Deactivate the base environment
conda deactivate

# Activate the TensorFlow-GPU environment
conda activate tfgpu_env

# Start a Python session to verify that python 3.8 is in use
python

# Type CTRL-D to exit and deactivate the environment
conda deactivate

# -------------------------------------------------------------#

# For completeness, the list of Python imports is shown below:

import re
import pandas
from random import randint, uniform
from numpy import median
from numpy import argmax
from numpy import array
from numpy import array_equal
from keras.layers import Input
from keras.layers import LSTM
from keras.layers import Dense
from keras.models import Model
from keras.utils import to_categorical
```

## Installation

To install **lstm-lib**, it is sufficient cloning or copying its repository within a given directory (e.g., the home directory) and add its full path to the PYTHONPATH environment variable. This can be done permanently by modifying the .bashrc file, by adding the following line:

```
export PYTHONPATH=$PYTHONPATH:~/lstm-lib
```

Please, be sure to have execution rights for the ~/lstm-lib/lstmlib.py file. If not, you may change them with:

```
chmod 700 ~/lstm-lib/lstmlib.py
```

&nbsp;
