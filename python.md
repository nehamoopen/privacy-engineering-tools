


# Python packages for synthetic data

This is a list of python packages that deal with generating synthetic data. It is compiled mainly through searching in google and GitHub. Naturally, some packages will be missed, so feel free to suggest other packages and make a pull request.

The python packages are subdivided into three different categories: tabular, purely generative and other. This is a loose classification, since packages might fall into multiple categories.



## Tabular datasets

This packages in this category are useful if you have a tabular dataset and want to create a new synthetic dataset with similar properties.


| Name | Methods |  Extra Features | Synthetic spectrum | Maintenance | GitHub stars | Developers | Paper | License |
|--|--|--|--|--|--|--|--|--|--|
| [SDV](https://github.com/sdv-dev/SDV) | Copula, GAN, TVAE | Single table, relational database, time-series, deidentification | synthetically-augmented replica | Active | 918 | MIT/DataCebo | [paper](https://dai.lids.mit.edu/wp-content/uploads/2018/03/SDV.pdf) | MIT | 
| [ydata-synthetic](https://github.com/ydataai/ydata-synthetic) | GAN | Single table and time-series | Synthetically-augmented multivariate plausible | Active | 691 | - | - | [MIT license](https://github.com/ydataai/ydata-synthetic/blob/dev/LICENSE) |
| [Gretel Synthetics](https://github.com/gretelai/gretel-synthetics) | LSTM | Differential Privacy | Synthetically-augmented multivariate plausible | Active | 281 | Gretel.ai | -| [Apache-2.0 license](https://github.com/gretelai/gretel-synthetics/blob/master/LICENSE) |
| [DataSynthesizer](https://github.com/DataResponsibly/DataSynthesizer) | Bayesian Network | Web User Interface, intermediate file, differential privacy | synthetic structural, synthetically-augmented plausible, synthetically-augmented multivariate plausible | Active | 166 | - | [paper](https://github.com/DataResponsibly/DataSynthesizer/blob/master/docs/cr-datasynthesizer-privacy.pdf) | MIT |
| [synthia](https://github.com/dmey/synthia) | fPCA, Gaussian copula, vine copula | Supports xarray | Synthetically-augmented multivariate/univariate plausible| Active | 27 | - | [software](https://doi.org/10.21105/joss.02863), [application](https://doi.org/10.5194/gmd-14-5205-2021) | MIT |


## Generative

Generative methods generally do not need any input dataset. Instead the user specifies the properties of the dataset and the package generates the synthetic data from this specification.

| Name | Creates | Extra features | Maintenance | GitHub stars | Developers | paper | License |
|--|--|--|--|--|--|--|--|
| [scikit-learn](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.make_regression.html#sklearn.datasets.make_regression) | Random matrices | - | Active | 50.6K | - | - | BSD-3-Clause |
| [faker](https://github.com/joke2k/faker) | Many kinds of private information | Modular structure | Active | 14.4K | - | - | MIT |
| [mimesis](https://github.com/lk-geimfari/mimesis) | Many kinds of private information | High performance, multilingual | Active | 3.6k | - | - | MIT |
| [plait.py](https://github.com/plaitpy/plaitpy) | User defined data | From user-defined template with statistical properties | Inactive | 418 | - | - | [MIT license](https://github.com/plaitpy/plaitpy/blob/master/LICENSE.txt) |
| [Synthdet](https://github.com/Unity-Technologies/SynthDet) | Images for object detection | - | Active | 287 | Unity Technologies | [paper](https://blogs.unity3d.com/2020/09/17/training-a-performant-object-detection-ml-model-on-synthetic-data-using-unity-computer-vision-tools/) | Apache v2.0|
| [BlenderProc](https://github.com/DLR-RM/BlenderProc) | Images for segmentation, distance estimation  |  Physics simulation, camera sampling | Active | 1.5K | German Aerospace Center | [paper](https://arxiv.org/abs/1911.01911) | GPL-v3 |
| [pydbgen](https://github.com/tirthajyoti/pydbgen) | SQL databases and DataFrames  with private information | ease of use | Inactive | 232 | T. Sarkar | - | MIT |
| [timeseries-generator](https://github.com/Nike-Inc/timeseries-generator) | Time-series | GUI, built-in economics factors | Active | 63 | Nike | - | Apache 2.0 |
| [physim-dataset-generator](https://github.com/cmitash/physim-dataset-generator) | Images for object detection | 3D rendering | Inactive | 60 | - | [paper](https://arxiv.org/pdf/1703.03347.pdf) | [BSD-2-Clause license](https://github.com/cmitash/physim-dataset-generator/blob/master/LICENSE) |
| [google-semantic-location-history](https://github.com/UtrechtUniversity/google-semantic-location-history) | Google semantic location histories | - | Active | 2 | Utrecht University | - | MIT |

## De-identification
| name | De-identifies | Extra features | Maintenance | GitHub stars | Developers | paper | License |
|--|--|--|--|--|--|--|--|
| [presidio](https://github.com/microsoft/presidio) | Text and Images | customization | Active | 1.7K | Microsoft | - | MIT
| [deduce](https://github.com/vmenger/deduce) | Dutch medical texts | - | Active | 39 | V. Menger | [paper](https://www.sciencedirect.com/science/article/abs/pii/S0736585316307365) | GPL-v3
| [Masked-Piper](https://github.com/WimPouw/TowardsMultimodalOpenScience) | People in videos | kinematic overlays, time-series | Active | 2 | W. Pouw | - | - |
| [anonymoUUs](https://github.com/UtrechtUniversity/anonymouus) | Text | Pattern matching, directories | Active | 2 | Utrecht University | - | MIT |


## Specific use-cases

| name | Creates | Extra features | Maintenance | GitHub stars | Developers | paper | License |
|--|--|--|--|--|--|--|--|
| [syndata-generation](https://github.com/debidatta/syndata-generation) | Images for object detection | - | Inactive | 252 | - | [paper](https://arxiv.org/abs/1708.01642) | MIT |
| [smogn](https://github.com/nickkunz/smogn) | Improved tabular dataset | Synthetic Minority Over-Sampling, Pure Python | Active | 189 | N. Kunz | [paper](http://proceedings.mlr.press/v74/branco17a/branco17a.pdf) | GPL v3 |
| [mtt-distilation](https://github.com/GeorgeCazenavette/mtt-distillation) | Images for Machine Learning | Distillation from bigger to smaller dataset | Active | 184 | - | [paper](https://georgecazenavette.github.io/mtt-distillation/) | MIT
| [doppelGANger](https://github.com/fjxmlzn/DoppelGANger) | Timeseries generation | Use GANs, high customization | Active | 181 | - | [paper](https://arxiv.org/abs/1909.13403) | [BSD-3-Clause-Clear license](https://github.com/fjxmlzn/DoppelGANger/blob/master/LICENSE) |
| [augraphy](https://github.com/sparkfish/augraphy) | Paper documents | - | Active | 59 | Sparkfish | - | MIT |
| [tofu](https://github.com/spiros/tofu) | UK Biobank synthetic data | - | Inactive | 30 | - | - |  [paper](http://doi.org/10.5281/zenodo.3634604) | No License |
