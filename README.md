# genome_treatment

This is a R pacakge including some tools to treat aligned genome sequence.

To acess them, you can try 
   
     library(devtools)
     install_github("wuaipinglab/genome_treatment/findout")
     library(findout)
     ?findout::findout_mutation()

# 1. findout 

This is developed for SARS-CoV-2.
 
Now the available package is: 
 
#   1.1 findout_mutation (depending on tidyr, stringr)
      
   Description: When you try to call INDEL or SNP from a very large and already aligned geonome sequences on your local system, I will recommend you to use it.
      To use it try: 
       
      findout_mutation(filename,key_pattern)
     
# Parameters:

filename: The file name of your aligned sequences.

key_pattern: An unique pattern in your refference sequence in the above aligned file, such as a EPI id.

As a quality control, sequences will be removed with more than 15 "N" or 50 other degenerate bases like "R".

# Good Luck


