# Introduction to SQL for Data Science (Spring 2019)

The Visualization Core Lab will host an *Introduction to SQL for Data Science* workshop on **Thursday, 2 May 2019 in Auditorium 0215 (between buildings 4 and 5)**. Visualization lab staff will provide an introduction to SQL for data science designed for learners with little or no previous experience with SQL programming. Topics covered will include the following.

* Selecting data 
* Sorting and removing duplicates
* Filtering
* Calculating new values
* Missing data
* Aggregation
* Combining data
* Data hygiene
* Creating and modifying data
* Programming with databases-Python
* Programming with databases-R
* Next steps for more advanced SQL training for data science.

**This is a live-coding based workshop and learners are expected to bring their own laptops with the required software already installed.**

## Schedule Overview 

The workshop will largely follow the [The Carpentries](https://carpentries.org/) [Databases and SQL lecture materials](http://swcarpentry.github.io/sql-novice-survey/).

* Instructors will be available between 8:30-9:00 am to help with software setup.
* Morning session (9:00 am -12:00 pm) with coffee break at 10:30 am.
* Afternoon session (1:00 pm - 5:00 pm) with coffee break at 3:00 pm.

## Installation Instructions

SQLite is included as part of the standard Python library so as long as you have Python installed on your machine you should be able to complete most all of the workshop without any further installation.

Check whether or not you have [SQLite](https://www.sqlite.org/index.html) installed on your local machine by running the following command in a terminal.

```bash
$ which sqlite3
```

If you are running Windows, then run the following command in a command prompt.

```
$ where sqlite3
```

### Git
In order to clone the workshop repository containing the database file and additional materials you will need to install Git.

You can check whether or not you have [Git](https://git-scm.com/) already installed on your local machine by running the following command in a terminal.

```bash
$ which git
```

If you are running Windows, then run the following command in a command prompt.

```
$ where git
```

If necessary install [Git](https://github.com/kaust-vislab/introduction-to-git-for-data-scientists#installation-instructions) and then [clone the workhsop repository](https://help.github.com/en/articles/cloning-a-repository) on your local machine. To clone this repository open a terminal (or Git Bash shell if you are running Windows), change the current working directory to the location where you want to create the clone of this repository and then run the following command in the terminal.

```bash
git clone https://github.com/kaust-vislab/introduction-to-sql-for-data-science.git
```

### Conda
In order to build the software environments for using SQL databases from Python and/or R you will need to have the [Conda](https://docs.conda.io/en/latest/) package management system installed on your machine.

To check whether the Conda is installed on your local machine by running the following command in a terminal.

```bash
$ which conda
```

If you are running Windows, then run the following command in a command prompt.

```
$ where conda
```

If Conda has not been installed on your machine, then install the Python 3 version of [Miniconda](https://docs.conda.io/en/latest/miniconda.html) from Anaconda for your OS. Once you have installed Conda on your machine run the following commands in make sure that you have the most recent patches.

```bash
$ conda update -y conda
$ conda init
```

Once Conda has been installed, then you can create and activate the appropriate software environment for the workshop. Python users should run the following commands in the terminal.

```bash
$ cd introduction-to-sql-for-data-science
$ conda env create -f python/environment.yml
$ conda activate introduction-to-sql-for-data-science-python
```

R users, meanwhile, should run the following commands in the terminal.

```bash
$ cd introduction-to-sql-for-data-science
$ conda env create -f r/environment.yml
$ conda activate introduction-to-sql-for-data-science-r
```

When you are done with this workshop you can deactivate the Conda environment by running the following in ther terminal.

```bash
$ conda deactivate
```

## Additional SQL Training Resources

Assorted links to additional resources for SQL training.

### Code Academy
* [Learn SQL](https://www.codecademy.com/learn/learn-sql)

### Udacity
* [SQL for Data Analysis](https://www.udacity.com/course/sql-for-data-analysis--ud198)

### O'Reilly
* [PostgreSQL: Up and Running (3rd edition)](http://shop.oreilly.com/product/0636920052715.do) [(Full Text Online)](https://www.safaribooksonline.com/library/view/postgresql-up-and/9781449373184/?ar&orpq)

### Core Data Science tools

In addition to knowledge of SQL, an aspiring data scientist you should seek to develop proficiency in the following areas:

* Proficiency in at least one of [Python](https://www.python.org/) or [R](https://www.r-project.org/about.html) (increasingly [Julia](https://julialang.org/))
* Version control using [Git](https://git-scm.com/) and either [GitHub](https://github.com/) or [GitLab](https://about.gitlab.com/).
* The Unix shell for interacting with clusters either locally at KAUST (i.e., Ibex, Nesser, Shaheen, etc) or in the cloud ([GCP](https://cloud.google.com/), [AWS](https://aws.amazon.com/), [Azure](https://azure.microsoft.com/en-us/), etc)
* Container-based work flows using [Docker](https://www.docker.com/) to enable your data science pipelines to run on your laptop, on cluster, even on HPC (without changing your code!).

In addition to the SQL lessons that we will cover in the workshop, [The Carpentries](https://carpentries.org/) have excellent introductory materials on [Git](http://swcarpentry.github.io/git-novice), [Shell](http://swcarpentry.github.io/shell-novice), [Python](http://swcarpentry.github.io/python-novice-gapminder/), and [R](http://swcarpentry.github.io/r-novice-gapminder/), as well as a number of more [domain-specific data science lessons](https://datacarpentry.org/lessons/) that are built on this tool stack.
