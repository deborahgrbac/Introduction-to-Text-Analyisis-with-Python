This repository is founded on Constellate notebooks.

The original Jupyter notebooks repository was designed by the educators at ITHAKA's Constellate project. The project was sunset on July 1, 2025. This current repository  use and resuse Constellate notebooks as Open Educational Resources (OER), free for re-use under a Creative Commons CC BY License.
This repository, Constellate notebooks and this readme file reference to the Ithaka-Constellate repository, but have been modified by Deborah Grbac for internal use at Università Cattolica del Sacro Cuore di Milano, email: deborah.grbac@unicatt.it

How to create a copy of these notebooks:

These notebooks may be downloaded with your browser or cloned using git software.

Download these notebooks in your browser
Choose the green "<> Code" button at the top of the repository, then "Download ZIP."

Clone these notebooks using Git
If you have git installed on the command line, these notebooks may be cloned using: git clone https://github.com/deborahgrbac/Introduction-to-Text-Analyisis-with-Python

If you are using a Git Desktop or some other graphical user interface, choose "clone" and supply the URL for this repository: https://github.com/deborahgrbac/Introduction-to-Text-Analyisis-with-Python

Using the notebooks.
The notebooks are written with Python and compatible with JupyterLab as of July 1, 2025. For best compatibility, we recommend using these notebooks on a local installation of JupyterLab. They should also work well on notebook platforms that faithfully reproduce the Jupyter notebook standard. We share some additional possibilities below.

System specifications.
For best results, we recommend a system meeting these specifications:

* Python 3.13+
* 3.5+ GHz, 4-core CPU
* 16+ GB RAM
* 30+ GB Disk Space
* No GPU acceleration required
Recommended local machine solutions for using Jupyter notebooks, or alternatively a hosting solution.
Local solutions can be classified into either JupyterLab or Integrated Development Environments (IDE)s. It can be difficult to install JupyterLab, so we share some recommended methods below. An IDE can be a more flexible tool than JupyterLab, and we make some recommendations of suitable IDEs below as well.

Installing JupyterLab locally (the best solution)
These notebooks use the Jupyter notebook (.ipynb) standard created by Project Jupyter. Their JupyterLab software remains free and open source. It is the best platform for using these notebooks.

For beginners without command line experience, we recommend Project Jupyter's JupyterLab Desktop with traditional application installers for Windows, Mac, and Linux.

For those comfortable using the command line, we offer basic instructions for:

* Mac OS X
* Windows 10
  
Not recommended local JupyterLab installation methods.
Using Anaconda is not recommend  because it can be difficult to install, troubleshoot, and uninstall. Anaconda installs a large suite of data science tools; many are not necessary for using these notebooks. Moreover, Anaconda can be difficult to properly un-install which makes it hard to switch if you would like to use another solution.

A better solution is Miniconda, which installs far fewer applications on the machine. However, the difficulty of installing Miniconda is similar to JupyterLab by itself.

Using a local IDE for Jupyter notebooks.
If you are familiar with using the VS Code or Pycharm IDEs, they offer tooling for working with Jupyter notebooks. VS Code has native support for Jupyter notebooks. PyCharm is also a good solution for Jupyter notebooks. PyCharm has free version with basic Jupyter notebook support and a Pro version with advanced Jupyter notebook functionality that is free for teachers and students.

GPU compute is not necessary.
There is no need to prioritize a cloud environment with GPU access for using these notebooks. These notebooks do not use a GPU directly, preferring to use GPU computation through APIs which are usually easier, faster, and cheaper. If you plan to train models, then an environment with GPU access may make sense.

JupyterHub (the best solution).
Project Jupyter offers a cloud-based solution with integrated JupyterLab called JupyterHub. While this is the best solution, it is impractical for most users to run their own JupyterHub since it requires server management expertise. 

JupyterHub hosting through Hugging Face, Digital Ocean.
If you are technically savvy, Hugging Face Spaces and Digital Ocean offer relatively easy ways to get JupyterHub running on a server. Plan on spending about $10/month for persistent storage and basic compute. The downside to this approach is you will need to be prepared to troubleshoot any platform issues. It is always a good practice to back up your notebooks to your local machine or a git repository, but this is especially important if you are new to server management.

GitHub Codespaces IDE.
If you would like a full, cloud-based IDE, then GitHub Codespaces offers cloud access to VS Code which has support for working with Jupyter notebooks. Choose this option if you are familiar with VS Code and you would benefit from a tight integration with GitHub.

Not recommended cloud-based solutions (Google Colab).
Google Colab is a popular platform for using Jupyter notebooks because Google offers limited-access to GPU acceleration for model training. The Constellate notebooks do not include model training and do not require GPU acceleration. Instead, they use APIs to access GPU acceleration, which is often faster, easier, and cheaper.

Outside of its limited, free GPU access, Google Colab is inferior to other cloud-based Jupyter notebook solutions. The user interface and functionality is closed, non-standard, and difficult to use for file management. Moreover, it lacks support for basic notebook features, including:

* Markdown local file access (no local notebook linking, no local image rendering)
* Only one notebook at a time (no tabs for opening multiple notebooks)
* No command line access (in the free tier)
* Notebooks developed for Colab often only work in Colab, locking users into the environment. Google Colab's architecture violates the FAIR principles of scientific data management.

Deepnote is a useful platform for data science professionals with some advanced functionalities for working collaboratively and accessing data repositories. The additional features make it better for working data scientists than teachers and learners.

Binder is a free platform useful for demonstrating notebooks, but it has no persistent storage. The speed and availability are not reliable.

Conda.
The Conda package manager is usually part of an Anaconda solution, such as Anaconda Cloud, Anaconda, or Miniconda. It can be used from the command line, but there are also graphical ways to manage packages with Conda. See the particular documentation for the version of Anaconda you are using.

Common text analysis packages used in these notebooks
* gensim - Create word embeddings, topic models, and other natural language processing outputs using modern statistical machine learning.
* matplotlib - Create static, animated, and interactive visualizations in Python.
* nltk (Natural Language Tool Kit) - Work with over 50 corpora and lexical resources, such as Wordnet. Deploy a suite of text processing libraries for classification, tokenization, stemming, tagging, parsing, and semantic reasoning.
* numpy - Speed up scientific analysis, taking advantage of large, multidimensional arrays and matrices.
* pandas - Automate high-performance analysis of structured (tabular, multidimensional, potentially heterogeneous) and time series data.
* pillow - A successor project that forked the Python Image Library (PIL) repository, Pillow has been adopted as a replacement for the original PIL.
* pyLDAvis - Visualize and transform topic models created with Latent Dirichlet Allocation.
* spaCy - Analyze 70+ languages with trained pipelines for different language tasks, including support for transformers, word vectors, embeddings, named entity recognition, part-of-speech tagging, dependency parsing, and more.
* tesseract-ocr - Convert images and pdfs into plain text in over 100 languages.
* vaderSentiment - Extract the sentiment of a text with a lexicon and rule-based tool.
* wordcloud - Visualize document word frequencies in artistic, customizable word clouds.
* Package versions used for these notebooks
  There is no need to install every package. This would use up significant space on your computer and lead to conflicts between different package versions. If you have installed enough packages that conflicts are arising between various package versions, it is a good idea to start using virtual environments with venv or poetry. If you can't get packages to work well together, here are the versions we used to create these notebooks:

* beautifulsoup4==4.12.2 
* click==8.1.3
* gensim==4.3.1
* ipympl==0.9.3
* jupyter-ai==2.19.1
* jupyter-ai-magics==2.19.0
* jupyterlab-git==0.50.0
* matplotlib==3.8.4
* numpy >=1.16 nltk==3.9.1
* openai==1.51.0
* pandas >=2.0.3
* pillow==10.3.0
* pyarrow==14.0.1
* pyldavis==3.4.1
* pytesseract==0.3.10
* regex==2023.6.3
* requests==2.32.3
* scikit-learn==1.5.1
* scipy==1.11.1
* seaborn==0.12.2
* spacy==3.5.4
* urllib3==2.2.2
* vadersentiment==3.3.2
* wordcloud==1.9.2
* zipp==3.19.2

You can find the original Constellate repository at: https://github.com/ithaka/constellate-notebooks and a selection of class videos on our Youtube channel https://www.youtube.com/@Constellate_org that go with the notebooks.

Languages
Jupyter Notebook
100.0%


NB: To read the full Constellate project readme file please go to the original repository: https://github.com/ithaka/constellate-notebooks.
