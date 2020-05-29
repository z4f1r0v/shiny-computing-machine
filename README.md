# Shiny Computing Machine
You like Scala and you want to do some exploratory data analysis (EDA)? 
You want to find the quickest way to get you on par with your python, pandas and matplotlib fellows?

Look no futher, my dear - the shiny computing machine is here!

So what does one need to do fast iterative data exploration?
In my mind the necessary steps are:
- data processing - enables ingesiton of data from any source and allows for conversion into a format that can be passed to an SQL engine
- SQL engine - enables issuing queries about your data given that it already is in the right format
- visualization - gives visual representaitons that aid the understanding of the numerical results
- documentation - gives the ability to supplement the provided analysis with explanations in natural language

## What's inside?
- Spark 
  - robust and elegant APIs that give you the ability to ingest and manipulate data from any relevant source or format
  - seemless converstion between powerful abstractions and SQL
  - ability to import custom Scala code
- Scala
  - functional programming
  - mature ecosystem
  - typesafety
- Plotly
  - interactive embedded graphs that allow for dynamic zooming, export and navigation
- Notebooks
  - fast iterative interaction with the data
  - IDE like capabilities
  - Markdown

## How to set it up?
1. Install [almond](https://almond.sh/) - I used docker for this task - `docker run -it --rm -p 8888:8888 almondsh/almond:latest`
2. Open the `127.0.0.1/...` link presented in the terminal once you start almond
3. Drag and drop the `.ipynb` notebook in this repo to the folder structure in your browser and upload your file
4. Open the notebook, adjust to your linking and start exploring

## Example
As a real world example I have spent some time exploring a dataset of a Danske Bank account. The two simple questions that I got answers to are:
- what's the overall trend of the transactions in for the whole dataset
- what are the most expensive transactions per year and month in the dataset

If you feel like you want to explore your data simply:
- save a given period as a CSV file with comma as a separator (otherwise you need to set the separator explicitly in the spark code to whatever you choose)
- import the file and the `.ipynb` in the root of the folder structure that you find when navigating to localhost the address to which you will find when you start the docker container
 
