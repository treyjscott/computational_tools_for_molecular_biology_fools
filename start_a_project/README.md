# 1. Starting a project

The advice in this section does not need to be taken all that seriously. There are multiple ways to start and organize a project.

### Project organization

The way I organize projects, is create a single project directory (Fig 1). Within this directory, I then create subdirectories for important data, code, or specific analyses.

![Fig 1](https://github.com/treyjscott/computational_tools_for_molecular_biology_fools/blob/main/static/img//directory_layout.png)

I keep all code in a single directory (scripts), but this can also get messy. An alternative is to keep code for specific analyses within their respective directories.

My brain works in R, so I organize everything with an R project. This allows me to write code and run some analyses in RStudio.

### Interface between local computer and cluster

I create the above directory structure on my local computer. Large data sets and analyses are performed on the [cluster](https://docs.rc.fas.harvard.edu/kb/running-jobs/), but small things are sometimes done locally (most phylogenetics or file parsing). 

Large data sets should be stored in appropriate places on the cluster (where they will not be purged). When you actually perform intense computations, you should use a scratch directory (/n/netscratch/bellono_lab/Lab/). Scratch directories are purged so it is not a place to keep things permanently. 

I keep important outputs in my local directories after they finish running on the cluster. To transfer files from the cluster to my local machine, I use [FileZilla](https://docs.rc.fas.harvard.edu/kb/sftp-file-transfer/), but [rsync](https://docs.rc.fas.harvard.edu/kb/rsync/) can also be used.


