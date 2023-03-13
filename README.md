# Linked Art Exhibition Browser Data Analysis 

The Linked Art Exhibition Browser Data Analysis is used to examine the 'shape' of exhibition data expressed as Linked Art JSON-LD.

The application includes Jupyter notebooks that can be viewed via various means, including via a web app interface using [Mercury](https://github.com/mljar/mercury).

The app was created for use with the [Linked Art Exhibition Browser](https://github.com/tgra/Linked-Art-Exhibition-Browser) and the [Linked Art Exhibition MoMA dataset](https://github.com/tgra/Linked-Art-Exhibition-Browser-MoMA-dataset).

This repository also contains notebooks that create summary data files for us with the [Linked Art Exhibition Browser](https://github.com/tgra/Linked-Art-Exhibition-Browser)

## Jupyter notebooks

### Data variables file 
- [data variables file](variables.ipynb) - A Jupyter notebook that defines variables that are reused in other notebooks. This notebook needs to be executed before the other notebooks, to initialise these variables.

### Data analysis


### Summary data file creation
- [exhibition summary file creator](exhibition_summary.ipynb)
- [person summary file creator](person_summary.ipynb)
- [person linked data](person_linkeddata.ipynb) - queries wikidata for image files and writes URLs to data/wikidata files


## How to view the notebooks 


###  Visual Studio Code - Jupyter plugin
https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter 

If you have the Jupyter notebook extension, you can run the notebooks in Visual Studio Code editor:
- open and run the `variables.ipynb` notebook
- open and run the `persons.ipynb` notebook

### Jupyter Notebook
https://jupyter.org/ 


The run the Jupyter notebook in the browser, use the following command:
- `jupyter notebook`
- open and run the `variables.ipynb` notebook
- open and run the `persons.ipynb` notebook
  


### Mercury
https://github.com/mljar/mercury

Mercury provides a web app interface to the Jupyter notebooks. 

- To start Mercury enter on the command line: 
- `mercury watch variables.ipynb` 
- This will start Mercury. 
- 
- To add notebooks to the web app, enter the following in the command line 
 
 `mercury watch person.ipynb `
  `mercury watch person_nationality.ipynb `
 ` mercury watch person_name.ipynb `
` mercury watch person_born.ipynb `
`  mercury watch person_exhibitions.ipynb `
 ` mercury watch exhibitions_year.ipynb `
 ` mercury watch exhibitions.ipynb`
  

Use the command `mercury list` to list the notebooks available in the app.

Use the commend `mercury delete <notebook filename>` to remove a notebook from the mercury web app


- Navigate to the URL provided e.g. http://127.0.0.1:8000/
- Importantly, first action should be to open the `variables` notebook and press `run`.
- Click on the Mercury logo to return to the home page
- You are now ready to view the other notebooks available

### Person
[person.ipynb](person.ipynb)

This notebook contains two interactive widgets that allow you to change input values to the notebooks

- birth year 
  - updates the `Selected birth year / first letter of surname` histogram
- nationality 
  - updates the `Selected nationality - American / Birth year` histogram

Enter a valid nationality or birth year and press `run` to view an updated output.

### Person - Nationality
[person_nationality.ipynb](person_nationality.ipynb)

### Person - Name
[person_name.ipynb](person_name.ipynb)

### Person - Exhibitions
[person_exhibitions.ipynb](person_exhibitions.ipynb)

### Person - Birth Date
[person_born.ipynb](person_born.ipynb)

### Exhibition
[exhibitions.ipynb](exhibitions.ipynb)

### Exhibition year
[exhibition_year.ipynb](exhibition_year.ipynb)

## Links

- Mercury  https://github.com/mljar/mercury
- Mercury documentation https://mercury-docs.readthedocs.io/en/latest/
- Jupyter notebooks https://jupyter.org/
- Linked Art https://linked.art
- [Linked Art Exhibition Browser](https://github.com/tgra/Linked-Art-Exhibition-Browser) 
- [Linked Art Exhibition MoMA dataset](https://github.com/tgra/Linked-Art-Exhibition-Browser-MoMA-dataset)