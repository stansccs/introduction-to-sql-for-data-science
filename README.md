# Introduction to SQL for Data Science

The Visualization Core Lab will host an *Introduction to SQL for Data Science* workshop on **Thursday, 2 May 2019 Auditorium 0215 (between buildings 4 and 5)**. Visualization lab staff will provide an introduction to SQL for data science designed for learners with little or no previous experience with SQL programming. Topics covered will include the following.

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

## Installation Instructions

If you have not already done so, install [Git](https://github.com/kaust-vislab/introduction-to-git-for-data-scientists#installation-instructions) and then clone the workhsop repository on your local machine by typing the following commands into a terminal (Mac OS or Linux) or Git Bash shell (Windows).

```bash
git clone https://github.com/kaust-vislab/introduction-to-sql-for-data-science.git
```

Installation instructions differ depending on whether you work primarily with Python or R (and thus will most likely use Python or R to interact with SQL databases in future work).

### Python
Check to see if you have the [Conda](https://docs.conda.io/en/latest/) package management system installed on your local machine by running the following command in a terminal.

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

Once Conda has been installed, then you can create and activate a software environment for the workshop by running the following commands in the terminal.

```bash
$ cd introduction-to-sql-for-data-science
$ conda env create -f environment.yml
$ conda activate introduction-to-sql-for-data-science
```

### R
If you have not already done so, [install both R and RStudio]() and then use the following commands to install required dependencies for the workhop.

```bash
r install.R
```

## Schedule Overview 

The workshop will largely follow the [The Carpentries](https://carpentries.org/) [Databases and SQL lecture materials](http://swcarpentry.github.io/sql-novice-survey/).

* Instructors will be available between 8:30-9:00 am to help with software setup.
* Morning session (9:00 am -12:00 pm) with coffee break at 10:30 am.
* Afternoon session (1:00 pm - 5:00 pm) with coffee break at 3:00 pm.

## Additional SQL Training Resources

Assorted links to additional resources for SQL training.

### Core Data Science tools

In addition to knowledge of SQL, an aspiring data scientist you should seek to develop proficiency in the following areas:

* Proficiency in at least one of [Python](https://www.python.org/) or [R](https://www.r-project.org/about.html) (increasingly [Julia](https://julialang.org/))
* Version control using [Git](https://git-scm.com/) and either [GitHub](https://github.com/) or [GitLab](https://about.gitlab.com/).
* The Unix shell for interacting with clusters either locally at KAUST (i.e., Ibex, Nesser, Shaheen, etc) or in the cloud ([GCP](https://cloud.google.com/), [AWS](https://aws.amazon.com/), [Azure](https://azure.microsoft.com/en-us/), etc)
* Container-based work flows using [Docker](https://www.docker.com/) to enable your data science pipelines to run on your laptop, on cluster, even on HPC (without changing your code!).

In addition to the SQL lessons that we will cover in the workshop, [The Carpentries](https://carpentries.org/) have excellent introductory materials on [Git](http://swcarpentry.github.io/git-novice), [Shell](http://swcarpentry.github.io/shell-novice), [Python](http://swcarpentry.github.io/python-novice-gapminder/), and [R](http://swcarpentry.github.io/r-novice-gapminder/), as well as a number of more [domain-specific data science lessons](https://datacarpentry.org/lessons/) that are built on this tool stack.
