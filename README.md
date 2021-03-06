# GoTermFinder
GoTermFinder was developed in Princeton University. It is used to perform GO term enrichment analysis. See details in: 
A web server of GoTermFinder is available at : https://go.princeton.edu/cgi-bin/GOTermFinder.

# How to run
First download the GOEnrich.zip file and unzip it. Example scripts and data for running GO enrichment is provided.
## 1. Start a server by running the following command
```bash
sh human_startGOserver_BP_2018.sh
```
## 2. Run GO enrichment for a user-provided gene list
```bash
perl geneset2go.pl example_genelist.txt 
```
The code above will generate enrichment results with file name suffix being _goea.table.

This example is for humans. If you would like to perform analysis for another organism, just change the gene ann    otation file in the human_startGOserver_BP_2018.sh code.

##############
## Note  #####
##############
### 1. Make sure that the server ID (15000 in this example) in the geneset2go.pl code is the same as that set in the human_startGOserver_BP_2018.sh code.
### 2. If the server ID does not work, change it to any other integer.
