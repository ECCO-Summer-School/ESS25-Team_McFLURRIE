## Files and folders in your project repository - to be deleted

This template provides the following suggested organizaiton structure for the project repository, but each project team is free to organize their repository as they see fit.

* **`contributors/`**
<br> Each team member can create their own folder under contributors, within which they can work on their own scripts, notebooks, and other files. Having a dedicated folder for each person helps to prevent conflicts when merging with the main branch. This is a good place for team members to start off exploring data and methods for the project.
* **`notebooks/`**
<br> Notebooks that are considered delivered results for the project should go in here.
* **`scripts/`**
<br> Code that is shared by the team should go in here (e.g. functions or subroutines). These will be files other than Jupyter Notebooks such as Python scripts (.py).
* `.gitignore`
<br> This file sets the files that will be globally ignored by `git` for the project. (e.g. you may want git to ignore temporary files or large data files, [read more about ignoring files here](https://docs.github.com/en/get-started/getting-started-with-git/ignoring-files))
* `environment.yml`
<br> `conda` environment description needed to run this project.
* `README.md`
<br> Description of the project (see suggested headings below)
* `model-card.md`
<br> Description (following a metadata standard) of any machine learning models used in the project

# McFLURRIE
## Mackenzie Freshwater Layers Uncover River Runoff Ice Evolution

### Collaborators

| Name | Personal goals | Can help with | Role |
| ------------- | ------------- | ------------- | ------------- |
| Marie Zahn | Gain experience running ECCOV4 and analyzing EMU outputs | Plotting ECCO output and Python  | Project Lead |
| Carenza Williams | Understand more about EMU analysis | ECCO model basics, Python code | Project Helper |
| Oceanne Bousquet | TBD | TBD | Project Helper |
| Mike Wood | TBD | TBD | Project Helper |

### The problem

Arctic freshwater is projected to increase over the next century. An increase in freshwater content in the Arctic may influence upper ocean stratification, in turn affecting upper ocean heat content and sea ice formation. We investigate the impact of a 10% increase in freshwater runoff on sea ice formation in the Fall at the mouth of the Mackenzie River.

## Data and Methods

### Data

These experiments were conducted using the Estimation the Circulation and Climate of the Ocean state estimate, version 4 release 5 (ECCOv4r5) (Ecco Consortium, https://ecco-group.org/products-ECCO-V4r4.htm). 

### Proposed methods/tools

We will run the ECCOv4r5 model in three different configurations: with the runoff increased by 10% globally; with the runoff increased by 10% only at the Mackenzie River; and with a time-varying, semi-realistic runoff globally. We will compare these outputs, which have daily frequency, with the base ECCOv4r5 run. Particularly, we will investigate the change in sea ice area, sea ice thickness, salinity, ocean heat content, and stratification at the mouth of the Mackenzie river. We are interested in analysing output from the years 2014-2019.

The causes of increases in salinity at the mouth of the Mackenzie river will be investigated using the ECCO Modelling Utilities (EMU) adjoint and convolution tools. 

## Project goals and tasks

### Project goals

We aim to answer (or be on the way to answering) the following questions:

* What is the impact of increased salinity on sea ice formation at the Mouth of the Mackenzie River?
* How much of this change is attributable to a change in runoff of the Mackenzie river alone, compared to a change in runoff globally?
* Why does this change in sea ice area occur?

### Tasks

What are the individual tasks or steps that need to be taken to achieve each of the project goals identified above? What are the skills that participants will need or will learn and practice to complete each of these tasks? Think about which tasks are dependent on prior tasks, or which tasks can be performed in parallel.

* Run three new ECCO model runs
* Analyse key diagnostics of these ECCO runs. In particular:
  * Sea ice area
  * Timing of sea ice onset
  * Sea surface salinity
  * Sea surface temperature
  * Sea ice thickness
  * Ocean heat content (upper 20m)
  * Ocean stratification (upper 20m)
* Run the EMU adjoint tool for each year of output.
* Run the EMU convolution tool for each year of output
* Analyse the results and consolidate understanding

## Project Results -- TBD

Use this section to briefly summarize your project results. This could take the form of describing the progress your team made to answering a research question, developing a tool or tutorial, interesting things found in exploring a new dataset, lessons learned for applying a new method, personal accomplishments of each team member, or anything else the team wants to share.

You could include figures or images here, links to notebooks or code elsewhere in the repository (such as in the [notebooks](notebooks/) folder), and information on how others can run your notebooks or code.
