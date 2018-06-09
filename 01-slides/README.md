![Pandas & Bokeh Logos](../imgs/logos_.jpg)

## "Adquirir, Manipular y Visualizar datos con Python: Pandas y Bokeh"

##### [Researcher on Paraphrase Detection on Spanish Text Corpora](http://menesesabad.com/scmc)

###### [Abel Meneses-Abad](https://www.linkedin.com/in/meneses-abad/) / [@abelma1980](https://twitter.com/abelma1980?lang=es)
________________________

##### Slides to Present in [PyDay Cienfuegos](), June 6th, 2018

##### Collaborator: [Leonel Salazar Videaux](http://debianhlg.cubava.cu/)
________________________

###### Get the [presentation](https://github.com/sorice/pbdata2018) source code.

###### Under [Attribution 4.0 International](http://creativecommons.org/licenses/by/4.0/) License.

---

### About the Speaker

- 2004 BSc on Telecommunications and Electronics
- 2005-09 Research on FLOSS Development & Deployment
- 2006-12 Team member of several software projects for high education: SistClon, Infodrez, Shakespeare and Sunshine.
- 2009 Chairman of Free Software Committee, Inform&aacute;tica-Habana 2009
- Member of the Cuban Free Technologies Users Group (GUTL)
- 2009-13 Dir. of Center for Studies of FLOSS for Culture
- From 2012 PhD candidate on Computing Science in the field of NLP

---

## What is all about?

- _python virtualenv_: preparing for real work!
- python-pandas __Acquisition__ & __Wrangling__ data.
- python-bokeh Data __Visualization__
  - Bokeh in jupyter notebooks
  - Deploying bokeh

---

#### Preparing the OS for python3 virtualenvs (using Debian 9, adjust for your own distribution)
```bash
$ apt install python3-venv python3-pip
```

#### Creating & activating the *pbdata* virtualenv
```bash
$ cd /to/your/projects/dir/
$ python -m venv pbdata
$ source pbdata/bin/activate
(pbdata)$
```
#### _Notice your __prompt__, now you are working __inside the pbdata virtualenv!__ _

#### Let the packages come in *offline mode*

```bash
(pbdata)$ pip install -i http://<my_IP_address>/pipdir pandas bokeh jupyter
```

```
Tips:
- It is a good practice to have every opened project in a root folder.
- pip is a mature tool allowing to work with an offline python packages repo.
```

--

### About virtualenv in python

> “Virtualenv creates a local environment with its own Python
> distribution installed.”

###### Practical Data Science CookBook (Tattar2017)

#### [Official & online virtualenvs docs](http://docs.python-guide.org/en/latest/dev/virtualenvs/#virtualenvwrapper)

#### Or go to *tutorial/venv.html* in your local python3-doc installation.

--

### Virtualenvs *allow you*

#### to ***test new*** python packages **without breaking the operating system**
#### to ***install python packages*** even **if you don't have root privileges**
#### to ***collaborate effectively*** with others **sharing the requirements**

---

### What are we doing?

![ML Sci Flow](../imgs/mlsciprocess_community.jpg)

--

### Loading, preprocesing & transforming data!

![ML Sci Flow](../imgs/mlsciprocess_community_a.jpg)

--

### Playing, learning & plotting!

![ML Sci Flow](../imgs/mlsciprocess_community_b.jpg)

---

### Python Pandas

*Test* your previous installation on ipython shell
```bash
(pbdata)$ cd 02-pandas-tutorial
(pbdata)$ ipython
```

*Do* something obvious

```python
In [1]: import pandas as pd
In [2]: df = pd.read_csv("data/titanic.csv")
In [3]: df.head()
```

--

### About Pandas

>“_Pandas_ provides high-level data structures and functions designed 
>to make working with structured or tabular data fast, easy, and 
>expressive.”
###### Python for Data Analysis, 2thE (McKinney2018).

#### Perfect for "Medium" Data: 5-100Gb

#### Where to learn pandas? Book [*Python for Data Analysis*](http://github.com/wesm/pydata-book). Wes McKinney (2018).
#### [Official & Online Doc](https://pandas.pydata.org/pandas-docs/stable/)
#### [Tutorial EuroSciPy 2017](https://github.com/jorisvandenbossche/pandas-tutorial)
#### Or go to your local python-pandas-doc installation.

--

## Pandas in action

Let's open pandas notebook inside folder **02-pandas-tutorial**.
###### Is the first notebook of the [EuroSciPy 2017 Pandas Tutorial](https://github.com/jorisvandenbossche/pandas-tutorial)

### Make sure you are in the _pbdata_ virtualenv! 

```bash
(pbdata)$ cd 02-pandas-tutorial
(pbdata)$ jupyter notebook
```

Let's work in the browser.

---

### The gap between pandas & bokeh
##### (some steps between wrangling & visualization)

* __Multidimensional Data Arrays__: *numpy* and *scipy.ndimage*
* __Data Statistical Analysis__: *statsmodels* and *scipy.stats*
* __Data Clustering or Classification__: *sklearn* and *scipy*

---

## Python Visualization

Preparing the virtualenv

```bash
(pbdata)$ pip install -i http://<my_IP_address>/pipdir matplotlib altair
``` 

*Test* bokeh installation and let's try a basic ploting example

```python
(pbdata)$ ipython

In [1] import bokeh
In [2] import pandas as pd
In [3] import matplotlib.pyplot as plt
In [4] pd.read_csv('data/iris.csv')
In [5] iris.plot(kind='hist', stacked=True, bins=20, alpha=0.5)
In [6] plt.show()
```

--

### About Bokeh

>"Bokeh is an interactive visualization library that targets modern web 
>browsers for presentation. Its goal is to provide elegant, concise 
>construction of versatile plots"

#### Where to learn bokeh?

#### [Bokeh Official & Online Doc](https://bokeh.pydata.org/en/latest/docs/gallery.html)
#### [Online tutorial](https://github.com/bokeh/bokeh-notebooks/)
#### [PyCon 2017 Tutorial](https://github.com/chalmerlowe/bokeh_tutorial)

--

### Bokeh in action

Let's open bokeh notebook inside folder **03-bokeh-tutorial**.
###### Is the first notebook of the [PyCon 2017 Bokeh Tutorial](https://github.com/chalmerlowe/bokeh_tutorial)

### Make sure you are in the _pbdata_ virtualenv! 

```bash
(pbdata)$ cd 03-bokeh-tutorial
(pbdata)$ jupyter notebook
```

Let's work in the browser again.

---

## Results

### You tell me!

---

## Closing remarks

* Python is *very* mature for science.
* Python is *very* mature for developing apps.
* Go *faster* using proven tools like virtualenv.
* *Share* and *learn* from people who also share.
