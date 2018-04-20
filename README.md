# ULL Practical 1
The code for all the tasks is in __[ULL-Practical1-EceTakmaz_BasakEskili.ipynb](https://github.com/ecekt/ULL-lab-1/blob/master/ULL-Practical1-EceTakmaz_BasakEskili.ipynb)__ 
(We have interactive visualizations with Bokeh for clusters, but GitHub may not show them through the browser.)


In the __[runs](https://github.com/ecekt/ULL-lab-1/tree/master/runs)__ folder, we provide the output files from the analogy task. We first give the question-answer pairs, then 5-most similar words to the estimated answer along with the cosine similarity between these words and the estimated answer. Then, we indicate the rank of the correct answer, first, keeping all the words in the ranking and then omitting the question words.


In the __[example_images](https://github.com/ecekt/ULL-lab-1/tree/master/example_images)__ folder, we provide some images that correspond to the clustering task, which we analyze in the report.


## Libraries

import numpy as np

import random


from scipy.stats import pearsonr

from scipy.stats import spearmanr

from scipy import spatial

from scipy import stats


from sklearn.metrics.pairwise import cosine_similarity

from sklearn.decomposition import PCA

from sklearn.cluster import KMeans

from sklearn.manifold import TSNE


import matplotlib.pyplot as plt


from mpl_toolkits.mplot3d import Axes3D


from bokeh.models import ColumnDataSource, LabelSet

from bokeh.plotting import figure, show, output_file

from bokeh.palettes import d3

from bokeh.io import output_notebook
