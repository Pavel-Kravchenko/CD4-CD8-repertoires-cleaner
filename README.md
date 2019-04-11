# CD4-CD8-repertoires-cleaner

This is a repo of CD4-CD8-repertoires-cleaner. 


This code is a part of lsfg TCR motive descovery project.

It filters CD4/CD8 tables after MIXCR (https://mixcr.readthedocs.io/en/master/). 

## Before you start

The pipeline is available only for <i>Linux</i> users </br>
Make sure that you have installed all components:
<ul>
<li>R and R-Studio with basic packages https://www.rstudio.com/
  <ul>
<li>```install.packages(c("data.table", "dplyr", "readr"))```
</ul>
</ul>


## Getting started

### Installation

First of all, you have to ```clone``` this directory</br></br>
```git clone https://github.com/Pavel-Kravchenko/CD4-CD8-repertoires-cleaner/```</br></br>
Then ```cd``` in CD4-CD8-repertoires-cleaner</br></br>
```cd CD4-CD8-repertoires-cleaner```</br></br>

Now you are ready to start.

If you like to clean a pair of files, you have to specify their names and the directory.
Your files should have a header like this in arbitrary order: 
```count	frequency	CDR3nt	CDR3aa	V	D	J	Vend	Dstart	Dend	Jstart```


For exaple command 
```Rscript files_cleaner_2.0.R as_Dv_PB_4.txt as_Dv_PB_8.c.txt `pwd` ./result/``` where `as_Dv_PB_4.txt` and  `as_Dv_PB_8.c.txt` are files to be cleaned, `pwd` is their directory, and `./result/` is the output dir.

Wait until the program is completed.

You are expected to receive a directory with cleaned and dropped clone files.

## Contact me

Feel free to contact me for any suggestions or critique.

Email: pavel-kravchenk0@yandex.ru 

Site: http://kodomo.fbb.msu.ru/~pavel-kravchenko/index.html 
