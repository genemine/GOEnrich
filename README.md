# GOEnrich

# start a server by running the following command
'bash
sh human_startGOserver_BP_2018.sh
' 
# run GO enrichment for a user-provided gene list
perl geneset2go.pl example_genelist.txt # this will generate enrichment results with file name suffix being _goea.tab    le.
 
##############
## Note  #####
##############
# 1. Make sure that the server ID (15000 in this example) in the geneset2go.pl code is the same as that set in the fi    rst step where server is started.
# 2. If the server ID does not work, change it to any other integer.
# 3. This example is for humans. If you would like to perform analysis for another organism, just change the gene ann    otation file in the human_startGOserver_BP_2018.sh code.
