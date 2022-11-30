[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-c66648af7eb3fe8bc4f294546bfd86ef473780cde1dea487d3c4ff354943c9ae.svg)](https://classroom.github.com/online_ide?assignment_repo_id=9066805&assignment_repo_type=AssignmentRepo)
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/27410/27410-group-assigment-group-1-nmn-production-with-e-coli/main)

# 27410 - Group assignment - Group 1 - NMN production with *E.coli*

> For this to work you will also have to keep `requirements.txt` up to date (by running `pip freeze > requirements.txt`).

## Project summary (<300 words)
The aim of the project is to design a cell factory for the production of NMN, a precursor of NAD, which taken as a supplement mitigates aging-induced diseases. Currently, its commercial production is through chemical synthesis, which makes it costly for the average consumer due to the complexity of its structure. This project considers three different pathways for the biosynthesis of NMN in _E. coli_ and studies how to optimize them.

Since _E. coli_ already has regulatory mechanisms to maintain NAD+/NADH levels, metabolic engineering is used to not only add new metabolic pathways, but also to make it more suitable for NMN production, avoiding inhibition and incorporating secretion into the media. In order to do this, the most comprehensive GSM of _E. coli_ is selected to work on, iML1515. After identifying the reactions involving NMN in the model, following literature, NAM, NA and NR are added as substrates, each for a different pathway. Their transporters and reactions into the cell are inserted, together with the missing parts of their pathways to produce NMN, as well as the extracellular transporter. Knockouts of pncC, ushA and nadR genes are performed due to literature recommendation too.

Several flux analyses are conducted, to confirm the intake of the new substrates for production of NMN, and to try to find a balance between biomass growth and NMN production. The three pathways present significant variation in NMN production, with the NR one obtaining an unexpectedly high biomass growth and yield of 11.9 mmol NMN/mmol Glucose, which means reaction boundaries might need more development. Algorithm simulations, such as OptGene and OptKnockout, are also run to find more knock-outs, knock-ins and media additions, optimizing the desired product and biomass accumulation while reducing by-products. These resulted in phenotypic phase plans (biomass vs NMN production graphs), but were not completed due to missing functions in package updates.

All in all, the regulation is in need of improvement for realistic results and reliable data to base research on.

## Project overview
The main information about the project can be read in the [Report notebook](https://github.com/27410/27410-group-assigment-group-1-nmn-production-with-e-coli/blob/160a3b5eaedd17a303472f80eb7cffa116dbc82a/Report.ipynb), in the main part of the repository. It contains the background for the project, our strategy, results and a discussion of them.
The scripts for the different analyses used to carry out the strategy of the project are in the [Scripts folder](https://github.com/27410/27410-group-assigment-group-1-nmn-production-with-e-coli/blob/160a3b5eaedd17a303472f80eb7cffa116dbc82a/scripts), along with other files necessary for them to work. These are referred to in the report. 
The [pictures folder](https://github.com/27410/27410-group-assigment-group-1-nmn-production-with-e-coli/blob/160a3b5eaedd17a303472f80eb7cffa116dbc82a/pictures) contains the figures used in the report, and a list of packages employed in the repository can be found in [requirements](https://github.com/27410/27410-group-assigment-group-1-nmn-production-with-e-coli/blob/160a3b5eaedd17a303472f80eb7cffa116dbc82a/requirements.txt)

