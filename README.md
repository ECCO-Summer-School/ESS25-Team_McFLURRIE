# McFLURRIE
## Mackenzie Freshwater Layers Uncover River Runoff Ice Evolution

<img src="McFLURRIE Logo.png" alt="" width="400"/>

### Collaborators

| Name | Personal goals | Can help with | Role |
| ------------- | ------------- | ------------- | ------------- |
| Marie Zahn | Gain experience running ECCOV4 and analyzing EMU outputs | Plotting ECCO output and Python  | Project Lead |
| Carenza Williams | Understand more about EMU analysis | ECCO model basics, Python code | Project Helper |
| Oceanne Bousquet | Learn to run ECCOV4, use EMU tools and visualize/analyze/interpret results | Python and understanding the mathematics behind EMU tools | Project Helper |

### The problem

Arctic freshwater is projected to increase over the next century. An increase in freshwater content in the Arctic may influence upper ocean stratification, in turn affecting upper ocean heat content and sea ice formation. We investigate the impact of a 10% increase in freshwater runoff on sea ice formation in the Fall at the mouth of the Mackenzie River.

## Data and Methods

### Data

These experiments were conducted using the Estimation the Circulation and Climate of the Ocean state estimate, version 4 release 5 (ECCOv4r5) (Ecco Consortium, https://ecco-group.org/products-ECCO-V4r4.htm). 

### Proposed methods/tools

We will run the ECCOv4r5 model in three different configurations: with the runoff increased by 10% globally; with the runoff increased by 10% only at the Mackenzie River; and with a time-varying, semi-realistic runoff globally (from JRA-55 reanalysis). The time-varying dataset provided lower rates of freshwater discharge in the Mackenzie River compared to the Fekete climatology. We will compare these outputs, which have daily frequency, with the base ECCOv4r5 run. Particularly, we will investigate the change in sea ice area, sea ice thickness, salinity, ocean heat content, and stratification at the mouth of the Mackenzie river. We are interested in analysing output from the years 2014-2019.

The causes of increases in salinity at the mouth of the Mackenzie river will be investigated using the ECCO Modelling Utilities (EMU) adjoint and convolution tools. 

## Project goals and tasks

### Project goals

We aim to answer (or be on the way to answering) the following questions:

* What is the impact of increased salinity on sea ice formation at the Mouth of the Mackenzie River?
* How much of this change is attributable to a change in runoff of the Mackenzie river alone, compared to a change in runoff globally?
* Why does this change in sea ice area occur?

### Tasks

Our project tasks include:

* Run four new ECCO model runs (control, 10% increase globally, 10% increase Mackenzie, time varying)
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

## Project Results

Exploration of the ECCO model output (control vs. perterbations) revealed small differences in sea ice area (<1%). However, more ice was generated for runs with increased freshwater (10% more) and less with decreased freshwater (i.e., time varying run). This is consistent with our hypothesis that increased freshwater would result in earlier/more ice formation due to increased stratification and less OHC in the surface layer.

We isolated a box near the Mackenzie River mouth (Lat bounds: 69, 72; Lon bounds: -143, -130) for our adjoint cost function of salinity (0-20m). From our convolution results, we found freshwater runoff modulates seasonal variability in salinity anomalies near the Mackenzie River mouth and wind stress controls interannual variability.

Future work could explore larger perterbations in freshwater discharge (>10%). From our preliminary results, we hypthesize increased freshwater results in greater sea ice area/volume, but does not change the timing of sea ice advance (i.e., onset).
