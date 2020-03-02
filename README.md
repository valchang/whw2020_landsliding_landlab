# whw2020_landsliding_landlab

## Project Title: Hydrologic controls on hillslope-to-channel sediment transport modeling in Landlab

## Collaborators on this Project:
•	Project Lead - Erkan Istanbulluoglu

•	Data Science Lead - Jeff Keck

## The Data Science Problem:
Coupled physical modeling of three processes: precipitation, hydrologic transport, landslides.

...sensitivitity of multiple time series input to the model...visualization of dynamic spatiotemporal processes across a hillslope scaled to a region. 

Participants on this project will build skills with: 

## The GeoScience Problem:

In this project, we will run a hillslope-to-channel sediment transport model using different precipitation and flow inputs. The purpose of the tutorial will be to (1) Investigate how different rates and patterns of hydrologic inputs change the output of the sediment transport model and (2) introduce the Landlab modeling environment, a python library of tools useful for conducting geomorphology experiments.
The sediment transport model consists of three individual models: a shallow landslide model that produces the sediment and is forced using a time series of precipitation; a debris flow runout model that transports the landslide material from the hillslope to the channel and is sensitive to flow in the channel; and finally a channel network sediment transport model that transports the debris flow material via bedload transport and is forced with a time series of flow. All three models are written as or in the process of being written as components of Landlab. Moreover, for all three components, sediment production/transport response to the hydrologic forcings is not well understood.
I will help users install Landlab and provide a Landlab model of a small basin pre-configured for each of the three sediment transport modeling components. As a group, we will brainstorm a series of questions to investigate and experiment. Example questions related to each module are listed below: 
The shallow landslide model can be run using a time series of precipitation or the precipitation can be generated from a user defined probability distribution of precipitation magnitude.


## Objectives:
In this project we will use a Landlab (Hobley et al., 2017) ....

Project domains ... 

Project will require developing ... 

A side project ideas ...

 Question 1: Does the pattern of precipitation affect model results; i.e. does antecedent precipitation affect model results. Question 2: If the mean of the precipitation probability distribution is the same, how does the type (i.e.: uniform vs lognormal) of the distribution affect shallow landslide rates? 
The mass wasting router tracks the landslide debris as a debris flow until either a slope threshold is met or the ratio of the channel flow to the volume of sediment is larger than a user defined threshold. Question 1: How does the channel flow to volume of sediment threshold affect the location of debris flow deposition?
Bedload transport in the channel network sediment transporter is a function of flow depth and the shear stress exerted by the flow on the sediment. Question 1: How does the method used to compute flow depth affect bedload transport? 
As we test model response to output, we will also develop plotting scripts. I can provide boiler plates and coding assistance to those first learning landlab.


## Sample Data Inputs  : 
• **Synthetic Model Dataset**:

Probability distribution of precipitation magnitudes.  

Hydrograph


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
