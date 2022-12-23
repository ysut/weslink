# weslink
__Under construction__ 🚧   
(EXCEL file is only available)

This notebook is to insert hyperlinks to HGMD, UCSC, and DECIPHER to your excel files. 
Please let me know if there are any bags.

When analyzing WES, we often deal with files that have been annotated with variants by annotation tools such as ANNOVAR.
Copy-pasting gene symbol is tedious, so I created a tool to insert links to web databases to your annotated excel files.

click here :arrow_lower_left:  
[![Open with Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ysut/weslink/blob/main/weslink_beta.ipynb)

## Usage
__Under construction__ 🚧

>**Warning**  
>Please note that the links to DECIPHER may contain errors associated with incorrect gene symbol and liftover.
  
You can choose columns that will be inserted hyperlinks.  
  
For example,   
the `hgmd_link` variable contains the column number where the URLs to the HGMD will be inserted.  
You can change this column number as you wish.  
  
Additionaly, if your Excel file does not have column `Gene.refGene`,  
change `Gene.refGene` to the name of the column containing the gene symbol.

~~~
hgmd_link = '1'
ucsc_link = '2'
franklin_link = '3'
decipher_link = '4'
symbol_column = 'Gene.refGene'
franklin_page = 'assessment-tools' 
is_hgmd = True
is_ucsc = True
is_franklin = True
is_decipher = True
ucsc_width: int = 30 
~~~
