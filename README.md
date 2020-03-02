# whw2020_landsliding_landlab

## Project Title: Hydrologic controls on hillslope-to-channel sediment transport modeling in Landlab

## Collaborators on this Project:
•	Project Lead - Erkan Istanbulluoglu

•	Data Science Lead - Jeff Keck

Available contributors and resources:  Christina Bandaragoda, Rhonda Strauch (remote; Seattle City Light)

## Development Reference for suggested sections

The problem
What water problem are you going to explore? Provide a few sentences. If this is a technical exploration of software or data science methods, explain why this work is important in a broader context.

Application Example
List one specific application of this work.

Sample data
If you already have some data to explore, briefly describe it here (size, format, how to access).

Specific Questions
List the specific tasks you want to accomplish or research questions you want to answer.

Existing methods
How would you or others traditionally try to address this problem?

Proposed methods/tools
Building from what you learn at waterhackweek, what new approaches would you like to try to implement?

Background reading
Optional: links to manuscripts or technical documents for more in-depth analysis.


## The Data Science Problem:
Coupled physical modeling of three processes: precipitation, hydrologic transport, landslides.

...sensitivitity of multiple time series input to the model...visualization of dynamic spatiotemporal processes across a hillslope scaled to a region. 
 
Add sizes of files, computer memory limits, model run time information.

## The GeoScience Problem:

In this project, we will run a hillslope-to-channel sediment transport model using different precipitation and flow inputs. The purpose of the tutorial will be to (1) Investigate how different rates and patterns of hydrologic inputs change the output of the sediment transport model and (2) introduce the Landlab modeling environment, a python library of tools useful for conducting geomorphology experiments.
The sediment transport model consists of three individual models: a shallow landslide model that produces the sediment and is forced using a time series of precipitation; a debris flow runout model that transports the landslide material from the hillslope to the channel and is sensitive to flow in the channel; and finally a channel network sediment transport model that transports the debris flow material via bedload transport and is forced with a time series of flow. All three models are written as or in the process of being written as components of Landlab. Moreover, for all three components, sediment production/transport response to the hydrologic forcings is not well understood.
I will help users install Landlab and provide a Landlab model of a small basin pre-configured for each of the three sediment transport modeling components. As a group, we will brainstorm a series of questions to investigate and experiment. Example questions related to each module are listed below: 
The shallow landslide model can be run using a time series of precipitation or the precipitation can be generated from a user defined probability distribution of precipitation magnitude.


## Objectives:

### If you want to build your physical process modeling skills with Python and Jupyter Notebooks, 
In this project we will use a Landlab (Hobley et al., 2017) .... to streamline the coupling of three compononents and test the sensitivity of climate forcings and hydrology to develop boundary conditions that are realistic. 

we have tutorials and startup examples and will be available all week to provide coding assistance to those first learning landlab.
 Question 1: Does the pattern of precipitation affect model results; i.e. does antecedent precipitation affect model results. Question 2: If the mean of the precipitation probability distribution is the same, how does the type (i.e.: uniform vs lognormal) of the distribution affect shallow landslide rates? 
The mass wasting router tracks the landslide debris as a debris flow until either a slope threshold is met or the ratio of the channel flow to the volume of sediment is larger than a user defined threshold. Question 1: How does the channel flow to volume of sediment threshold affect the location of debris flow deposition?
Bedload transport in the channel network sediment transporter is a function of flow depth and the shear stress exerted by the flow on the sediment. Question 1: How does the method used to compute flow depth affect bedload transport? 
As we test model response to output, we will also develop plotting scripts. I can provide boiler plates 

Invited contributions could include: interesting tutorials, reproducible models, better ways to design and explain how we build model experiments that couple multiple complex models.  



### If you have some coding experience 
and want to build modeling skills with Python and help us couple a hydrology model to a transport model... describe that challenge.. give a link to the Github repository that we want to develop

Is the network sediment transport and the mass wasting transporter realistic??  

Invited contributions could include: Advancing Landlab components, building new python scripts


###  If you want to experience working on supercomputers, help us on XSEDE.

we have a big compute program and the model takes a LONG time to run.   We need to test performance of the workflow at at 1000 km2 watershed scale. 

Invited contributions could include: test and share understanding on the limits of what we could compute and how to use cloud compute resources to do it.


## Sample Data Inputs  : 
• **Synthetic Model Dataset**:

Probability distribution of precipitation magnitudes.  

Hydrograph

• **Observed sediment transport**:

USGS data for bedload transport inferred from suspended data observations

• **Distributed Hydrologic Model Dataset**:

https://www.hydroshare.org/resource/f4a060f538184d49b642b7c079cbe0be/  has streamflow processed only for the links shown in this Google Map. 

A Google Map of links in the DHSVM digital network selected for streamflow output are available at:
https://www.google.com/maps/d/u/0/edit?mid=1z9yxQ6P_mPsu4NZyqP4Pj8OWJ1CGmi9R&ll=48.631435868567515%2C-121.51666349999999&z=9 

This folder has DHSVM Outflow files for historic and future https://www.hydroshare.org/resource/f16bdb504c6a4fb39e80ff1070a86704/ 

Inside is this file is only for the Sauk extent where we ran the temperature model 

[Click on this and it will download Sauk_1969-2001_biasLivneh_WRF_TH8-WhiteTH15_mu12.8_his/Outflow.Only.gz](
https://nam03.safelinks.protection.outlook.com/?url=https%3A%2F%2Fwww.hydroshare.org%2Fresource%2Ff16bdb504c6a4fb39e80ff1070a86704%2Fdata%2Fcontents%2FSauk_1969-2001_biasLivneh_WRF_TH8-WhiteTH15_mu12.8_his%2FOutflow.Only.gz&data=02%7C01%7Cpfeiffa%40wwu.edu%7C283eb67599ea41fa1b7f08d7b99d49a0%7Cdc46140ce26f43efb0ae00f257f478ff%7C0%7C0%7C637181958568260286&sdata=M3NUFpv5vqr4rQWTMUbIWjtaFiUmxKQLtw4b9fBJscU%3D&reserved=0)

I think this is what you are looking for.  We have more Skagit runs going on now with Ronda's landsliding updates, but that is for the entire Skagit Seattle City Light domain, not just Sauk. 


• **current climate**:

   

• **past climate**:


     
• **future climate**:

    - MACA data using Observatory for Gridded Hydrometeorology (OGH) - (https://climate.northwestknowledge.net/MACA/)

## References: 

• Hobley, D. E. J., J. M. Adams, S. S. Nudurupati, E. W. H. Hutton, N. M. Gasparini, E. Istanbulluoglu, and G. E. Tucker, (2017): Creative computing with Landlab: an open-source toolkit for building, coupling, and exploring two-dimensional numerical models of Earth-surface dynamics, Earth Surf. Dynam., 5: 21-46, doi:10.5194/esurf-5-21-2017.

• Livneh, B., E. A. Rosenberg, C. Lin, B. Nijssen, V. Mishra, K. M. Andreadis, E. P. Maurer, and D. P. Lettenmaier, 2013: A Long-Term Hydrologically Based Dataset of Land Surface Fluxes and States for the Conterminous United States: Update and Extensions. (2013). J . Climate, 26.  

• Livneh, B., Theodore J. Bohn, David W. Pierce, Francisco Munoz-Arriola, Bart Nijssen, Russell Vose, Daniel R. Cayan, & Levi Brekke (2015). Scientific Data 2. doi:10.1038/sdata.2015.42

• Phuong J., Bandaragoda C., Istanbulluoglu E., Beveridge C., Strauch R., Setiawan L., S. D. Mooney (2019).
Automated retrieval, preprocessing, and visualization of gridded hydrometeorology data products for spatial-temporal exploratory analysis and intercomparison, Environmental Modelling & Software.

• Add Strauch reference
