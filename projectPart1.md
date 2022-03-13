# Project Part 1

The goal of this part of the project is to get some familarity with how to approach a machine learning data science project. You will be working with the data science cookie cutter template. This will be an individual project but you will be exploring data sets you may eventually work with as part of your project.

## Overview of Steps

### Step 0: Keep Data out of Repo but everything else shoudl be there

**Warning:** Never commit large data files in a github repository.

It is important that you never commit large files into your repository. It is very very hard to delete files in a git repository. Sure, you can delete the file and commit it but a copy of the file ends up living in the hidden .git directory. You can't just delete it there. If you do you risk corrupting the whole repository. Instead you should use [.gitignore](https://git-scm.com/docs/gitignore), as in the blog post [Gitignore, What is it and How to Add to Repo](https://www.freecodecamp.org/news/gitignore-what-is-it-and-how-to-add-to-repo/). To manage large data file either use git  [Git Large File Storage](https://docs.github.com/en/repositories/working-with-files/managing-large-files/about-git-large-file-storage) if the size is under 2GB, or learn how to keep your data in dropbox, microsoft one drive or google drive and link (shortcut) the file to the repository. You still may need to download it separately but CCNY/CUNY have large storage allowances for one drive and dropbox in particular.

### Step 1: Keep all your work in a repo and commit often

Open a git repository using the classroom link. The template should be created for you using [Cookiecutter Data Science](https://drivendata.github.io/cookiecutter-data-science). You will need to manually go through the files and change some of the variable names. Follow the README.md. Please read the cookiecutter documentation and use the structure of the template for this project.

Keep in mind your experiments should go into the folder notebooks and your report should be in the reports folder. If you can factor out code that you will import into notebooks you should put that code in the src folder. Aagain read the [Cookiecutter Data Science](https://drivendata.github.io/cookiecutter-data-science) documentation.

**It is very important that you commit often. If there are not frequent commits I will have to assume the code was copied and pasted and you will recieve little credit. The work should show your thinking process over time and not just at the last minute**

### Step 2: Selecting Data

Here are a number of resources for finding data sets

#### General Data Set Aggregators

* [kaggle data sets](https://www.kaggle.com/datasets) and
* [kaggle challenges](https://www.kaggle.com/competitions)
* [awesome public data sets](https://github.com/awesomedata/awesome-public-datasets)
* [OpenML](https://www.openml.org/)
* [Datahub.io Collections](https://datahub.io/collections)
* [Paperswithcode Datasets](https://paperswithcode.com/datasets)
* [VisualData Discovery](https://visualdata.io/discovery)
* [Registry of Open Data on AWS](https://registry.opendata.aws/)
* [Google Datasets](https://datasetsearch.research.google.com/help)


#### Public government datasets

* [Data.gov](https://data.gov/)
* [Data USA](https://datausa.io/)
* [data.europa.edu](https://data.europa.eu/data/datasets?locale=en)
* [US Healthcare Data](https://researchguides.dartmouth.edu/c.php?g=517073&p=6289098)
* [US Education Data](https://nces.ed.gov/)
* [NYC Open Data](https://data.cityofnewyork.us/)
* [Los Angeles Open Data](https://data.lacity.org/)
* [Chicago Open Data](https://data.cityofchicago.org/)
* [Houston Open Data](https://data.houstontx.gov/)
* [UK Data Service](https://ukdataservice.ac.uk/)
* [UK Government Data](https://www.gov.uk/government/statistical-data-sets)
* [United Nations](https://data.un.org/)

#### Machine Learning Datasets for Finance and Econ

* [Financial Times](https://markets.ft.com/data/)
* [quandl](https://www.quandl.com/data)
* [IMF Data](https://www.imf.org/en/Data)
* [JPMorgan](https://www.jpmorganchase.com/en/investor/data-research/data-sets.html)
* [American Economic Association](https://www.aeaweb.org/resources/data/)
* [World Bank](https://data.worldbank.org/)

#### Image Datasets for Computer Vision

* [MIT CSAIL LabelMe](http://labelme.csail.mit.edu/Release3.0/browserTools/php/dataset.php)
* [Imagenet](https://image-net.org/)
* [Kinetics](https://deepmind.com/research/open-source/kinetics/)
* [LSUN: Construction of a Large-scale Image Dataset using Deep Learning with Humans in the Loop](https://paperswithcode.com/paper/lsun-construction-of-a-large-scale-image)
* [MSCOCO](https://paperswithcode.com/dataset/coco)
* [COIL-100](https://www1.cs.columbia.edu/CAVE/software/softlib/coil-100.php)
* [VisualGenome](http://visualgenome.org/)
* [Open Images Dataset](https://ai.googleblog.com/2016/09/introducing-open-images-dataset.html)
* [YouTube-8M](https://research.google.com/youtube8m/index.html)
* [Labeled Faces in the Wild](http://vis-www.cs.umass.edu/lfw/)
* [Indoor Scene Recognition](http://web.mit.edu/torralba/www/indoor.html)
* [xView](http://xviewdataset.org/)
* [CelebFaces](http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html)
* [Stanford Dogs Datasets](http://vision.stanford.edu/aditya86/ImageNetDogs/)
* [Places](http://places.csail.mit.edu/index.html)
* [CityScapes](https://www.cityscapes-dataset.com/)
* [CIFAR](https://www.cs.toronto.edu/~kriz/cifar.html)
* [Visual Question Answering Datasets (VQA)](https://visualqa.org/)
* [IMDB-WIKI](https://data.vision.ee.ethz.ch/cvl/rrothe/imdb-wiki/)
* [MPII Human Pose Dataset](http://human-pose.mpi-inf.mpg.de/#overview)
* [Google Open Images V5](https://ai.googleblog.com/2019/05/announcing-open-images-v5-and-iccv-2019.html)


#### Natural Language Processing Datasets

* [The Big Bad NLP Dataset](https://index.quantumstat.com/)
* [Enron Email Dataset](https://www.cs.cmu.edu/~enron/)
* [Google NGrams](https://archive.org/details/google_ngrams)
* [The Wikipedia Corpus](https://www.english-corpora.org/wiki/)
* [SMS Spam Collection Datasets](https://www.kaggle.com/uciml/sms-spam-collection-dataset)
* [Yelp Open Dataset](https://www.yelp.com/dataset)
* [Blog Authorship Corpus](https://www.kaggle.com/rtatman/blog-authorship-corpus)

#### Sentiment Analysis Datasets for Machine Learning

* [Multi-Domain Sentiment Dataset](https://www.cs.jhu.edu/~mdredze/datasets/sentiment/)
* [Stanford Sentiment Analysis](https://nlp.stanford.edu/sentiment/code.html)
* [Sentiment140](http://help.sentiment140.com/for-students/)
* [IMDB Movie Reviews Dataset](https://ai.stanford.edu/~amaas/data/sentiment/)
* [Twitter US Airline Sentiment](https://www.kaggle.com/crowdflower/twitter-airline-sentiment)
* [OpinRank Review Dataset Data Set](https://archive.ics.uci.edu/ml/datasets/opinrank+review+dataset)
* [Amazon Review Data](https://nijianmo.github.io/amazon/index.html)
* [Sentiment Lexicons for 81 Languages](https://www.kaggle.com/rtatman/sentiment-lexicons-for-81-languages)
* [Paper Reiviews](https://archive.ics.uci.edu/ml/datasets/Paper+Reviews)


#### Text Datasets for Natural Language Processing

* [Jepordy Datasets](https://www.j-archive.com/)
* [20 Newsgroups](http://qwone.com/~jason/20Newsgroups)
* [Legal Case Reports Data Set](https://archive.ics.uci.edu/ml/datasets/Legal+Case+Reports)
* [Microsoft Research WikiQA Corpus](https://www.microsoft.com/en-us/download/details.aspx?id=52419&from=http%3A%2F%2Fresearch.microsoft.com%2Fapps%2Fmobile%2Fdownload.aspx%3Fp%3D4495da01-db8c-4041-a7f6-7984a4f6a905)
* [Public Databases](https://www.gutenberg.org)

#### Audio Speech and Music Datasets for Machine Learning Projects

* [Common Voice](https://commonvoice.mozilla.org/en/datasets)
* [Google AudioSet](https://research.google.com/audioset/)
* [LibriSpeech](https://www.openslr.org/12/)
* [The Spoken Wikipedia Corpora](https://nats.gitlab.io/swc/)
* [VoxForge](http://www.voxforge.org/)
* [Free Music Archive (FMA)](https://github.com/mdeff/fma)
* [Ballroom](http://mtg.upf.edu/ismir2004/contest/tempoContest/node5.html)

#### Autonomoust Vehicles Datasets

* [Berkeley DeepDrive BDD100K](https://bdd-data.berkeley.edu/)
* [comma.ai driving dataset](https://archive.org/details/comma-dataset)
* [Oxford’s Robotic Car](https://robotcar-dataset.robots.ox.ac.uk/)
* [Laboratory for Intelligent & Safe Automobiles](https://cvrr.ucsd.edu/home)
* [Baidu ApolloScape: Dataset for Autnomous Driving](http://apolloscape.auto/)
* [Google-Landmarks-v1](https://ai.googleblog.com/2018/03/google-landmarks-new-dataset-and.html), [Google-Landmarks-v2](https://ai.googleblog.com/2018/03/google-landmarks-new-dataset-and.html)
* [PandaSet](https://scale.com/open-datasets/pandaset)
* [NuScenes](https://www.nuscenes.org/)
* [Open Waymo Dataset](https://waymo.com/open/)

### Step 3: Plan for you future project

Please use this refrerence in terms of your future project: [Stanford Univerisity\'s CS229](http://cs229.stanford.edu/projects.html). It also has some good discussion of what you might do for a project and where you may find data. Make sure that you are looking at a data set that is not a simple quick execise. This should not be a small data set like the titanic data set or the MNIST data set. It should either by large in terms of the number of data points (at least several thousand "rows") or large in the number of features. For example images and audio files are typically complex with many dimensions in terms of number of features.

Think about different hypothesis you could investigate on your data set. Take notes in a markdown file indicating the kind of hypothesis you expect to see when you look at your data. As you do EDA you should revisie these.

### Step 4: Data Wrangling, Data Cleaning, Preliminary EDA

How much missing data is there? Determine a prelimanary EDA to look at basic statistics and to see if there is to much missing data? What are the means, standard deviations, and other statisics on feaures. What happends when you filling in missing data will effects the statistics? There should be figures and discussion. Please use notebooks to do your analysis but when you submit, you must summerise your analysis. Do NOT just fill notebooks with output of some kind of runs without discussion or figures.

### Step 5: EDA and Data Visualization

Here you should show again the overall statistics of features or potential features. Besides summary statistics, you should be showing how potential features relate to each other using measures such as correlation or mutual information. One of your goals should be either regression or classification and you should explore what features are correllated with your target label or variable. This should be visible in the plots. Again, in your experimental notebooks this may be a bit disorganized, but there should be a notebook where the explanation is clearly spelled out and summerized. Whenever you make a run, take the time to explain not just what the figure is but what it ended up showing. Each diagram figure and result tells you something, explain what.

### Step 6: Invesigate some models and the importance of features. 

Here you should run classification models or/regression models to see how strong a signal there is in your data set. Your data should **always** have training, validation and testing data subsets. You should make your exploration based on the training and validation sets. The key question is, again what features and normalizations provide the strongets results from simple models such as KNN, linear models (eg logistic regression), and decision trees. You should pick the models appart, and generate some visualizations to understand exactly how these models do and why. To the extent that there is some data on which these models do not work well, you should discuss why by looking at the original data for those data and trying to determine if those points are special in anyother way.


### Step 7: Provide evaluation and conclusions

Your result should include peformance metrics, classification reports, accuracies, confusion matrices, and ROC curves. Again you should explain your results. If you have a model with high "accuracy" but unbalanced classes, then your accuracy is meaningless and you should balance first. Make sure you understand what is the reason for unbalanced false postives or false negatives, and how you can fix it. Again, when you present things do not just simply show but explain WHAT it shows and what the impact is. Commit all these into your repo and submit that repo to submission in blackboard.

