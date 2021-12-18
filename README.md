# master-thesis
## Dynamic Operator Selection for Dynamic Data Streams

### This repository contains the code for the Master Thesis. 

### The repository is structred as follows: 

#### 1. Notebooks named as DataDistributions-[]_save.ipynb contain the evaluation of sorting algorithms on different data distribution of different sizes. If you want to test them out just run the specific notebook you are interested in. They estimate and save the average runtimes of each algorithm on each distribution. After that those runtimes are dynamically loaded from other notebooks.

#### 2. The notebook PlotAllTogether.ipynb is a summary of the results in the previous results. You can directly run this notebook, as the results from the previous notebook are stored in the "DATA" folder and are dynamically loaded here. Here you can find plots of the sorting algorithms on each data distribution and each data size. 

#### 3. Notebooks named as Experiment_[]_Setting[].ipynb run experiments for the corresponding MAB-algorithm (Epsilon Greedy, UCB and Thompson Sampling) on the corresponding experimental artifical setting ranging from 1 to 5. You can run the corresponding file that you are interested in. The optimal solutions for the plots are extracted from the "DATA" folder and might not be the same on your machine.

#### 4. The notebook Plot_Experimental_Setting.ipynb plots the experimental synthetic datasets. 

#### 5. The notebooks Experiment_Functions.ipynb and Help_Functions_Experiments.ipynb contain help functions for the other notebooks.

#### 6. The notebook Run_all_MAB-1.ipynb runs each of the Experiment_[]_Setting[].ipynb Notebooks once. 

#### 7. The notebook Run_all_MAB_Together.ipynb runs five times the Run_all_MAB-1.ipynb notebook, i.e. contains the final results of the experimets on synthetic data. The file is archived, as it is very large otherwise. The results of the Thompson-Sampling method there are not official, as there was an error in the algorithm, so if you are interested specifically in the Thompson Sampling, you can find the results in the Run_all_TS_Updated.ipynb. 

#### 8. The Notebook Experiment_RandomSelection.ipynb contains the baseline solution of the synthetic experimental data.

#### 9. The Notebook Experiment_RealData.ipynb contains the generation of the real-world data set and the five runs of the MAB algorithms on the real data set. Important: The original real_world data set is not contained, as it is very large, you can find it at https://www.openml.org/d/42701 and once downloaded you can just run the notebook and it will create the modified version and run the experiment.

#### 10. The Notebook Experimet_RealData-OptimalSolution.ipynb caluclates the optimal solutions on the real world dataset.
#### 11. The file Rewards_Settings_Summary.xlsx contains the summary of the MAB approaches over synthetic, as well as real data. 

