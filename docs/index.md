
## How to convert a tab-deliminated file (.tsv/.txt) to csv

* #### Open your terminal  
    cd filedirectory

* #### Convert comma in the tsv file to semi-colon  
    perl -i.bak -pe 's/,/;/g' file.tsv

* #### Conver tab (\t) to comma(,)
    perl -i.bak -pe 's/\t/,/g' file.tsv

* #### The transformed data is saved in file.tsv  

* #### Rename the file.tsv to file.csv  

* #### The original tsv file backed up in file.bak  

