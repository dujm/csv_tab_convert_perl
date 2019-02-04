
## How to convert a tab-deliminated file (.tsv/.txt) to csv

* #### 1. Open your terminal  
    cd filedirectory

* #### 2. Convert comma (,) in the tsv file to semi-colon (;)
    perl -i.bak -pe 's/,/;/g' file1.tsv

* #### 3. Conver tab (\t) to comma(,)
    perl -i.bak -pe 's/\t/,/g' file1.tsv

* #### 4. The transformed data is saved in file.tsv  

* #### 5. Rename the file.tsv to file1.csv  

* #### 6. The original tsv file backed up in file1.bak



## How to convert a csv to tab-deliminated file (.tsv/.txt)  

* #### 2.2  Conver tab (\t) to semi-colon(;)
    perl -i.bak -pe 's/\t/;/g' file2.csv
    
* #### 3.2  Conver comma (,) to tab (\t)
    perl -i.bak -pe 's/,/\t/g' file2.csv
    
* #### 5.2 Rename the file.tsv to file2.tsv


