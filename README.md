# CD4-CD8-repertoires-cleaner
This is a repo of CD4-CD8-repertoires-cleaner.

This code is a part of lsfg TCR motive discovery project.

It filters CD4/CD8 tables after MIXCR (https://mixcr.readthedocs.io/en/master/).

</br>
## Before you start
The pipeline is available only for Linux users 
Make sure that you have installed all the components:
<ul>
<li>
R and R-Studio with basic packages https://www.rstudio.com/
<ul>
<li>```install.packages(c("data.table", "dplyr", "readr"))```
</ul>
</ul>
  
  </br></br>
  
# Getting started

## Installation
First of all, you have to clone this directory</br>

```git clone https://github.com/Pavel-Kravchenko/CD4-CD8-repertoires-cleaner/```

Then cd in CD4-CD8-repertoires-cleaner</br>

```cd CD4-CD8-repertoires-cleaner```


## Now you are ready to start.

If you like to clean a pair of files, you have to specify their names and the directory. 

Your files should have a header like this in arbitrary order: </br>
```count    | frequency |    CDR3nt    | CDR3aa |    V |    D |    J |    Vend |    Dstart |    Dend |    Jstart```</br>

And must have file name coding like `[disease or another flag]\_[donor or another flag]\_[tissue or another flag]\_[CD status or another flag]\_[experiment # or nothing].txt`

Examples:

as_Dv_PB_4.txt or as_Dv_PB_4_p2.txt
</br>

Command: 
```Rscript files_cleaner_2.0.R as_Dv_PB_4.txt as_Dv_PB_8.txt `pwd` ./result/``` </br>
where `as_Dv_PB_4.txt` and `as_Dv_PB_8.txt` are files to be cleaned, `pwd` is their directory, and `./result/` is the output dir.

Wait until the program is completed.

You are expected to receive a directory with cleaned and dropped clone files.

## Contact me
Feel free to contact me for any suggestions or critique.

Email: pavel-kravchenk0@yandex.ru

Site: http://kodomo.fbb.msu.ru/~pavel-kravchenko/index.html
