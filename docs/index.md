
### How to convert a tab-deliminated file (.txt/.tsv) to a csv?

* #### 0. Open the terminal  
    cd filedirectory

* #### 1. Convert file commas (,) to semi-colon (;)
    perl -pe 's/,/;/g' file1.txt > file2.txt

* #### 2. Conver tab (\t) to comma(,)
     perl -pe 's/\t/,/g' file2.txt > file3.csv
      
<br><br><br> 
### How to convert a csv to a tab-deliminated file (.txt/.tsv)?

* #### 1.  Conver file tabs (\t) to semi-colon(;)
    perl -pe 's/\t/;/g' file3.csv >file2.csv
    
* #### 2.  Conver comma (,) to tab (\t)
    perl -pe 's/,/\t/g' file2.csv > file1.txt


