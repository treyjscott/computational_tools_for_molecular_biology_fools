# 2. Installing packages

For most analyses, you will mostly use computer programs that are kep separate from the rest of your cluster activity (explained [here](https://www.anaconda.com/docs/getting-started/concepts/what-is-an-environment) for conda environments). This avoids conflicts between different software.

You will mostly use conda and singularity.

# Conda 

Before starting with conda you will need to load python (after logging into the cluster).

```
module load python
```

Once this is done, you should be able to type "cond" and then hit tab. If it autocompletes to "conda," then you successfully have conda (this autocopmlete trick is useful for knowing which programs are available and for finding out if certain files exist).

The basic steps for setting up a new conda environment are 1) create, 2) activate, and 3) install. The code below demonstrates by creating a conda environment for the alingment program [MAFFT](https://mafft.cbrc.jp/alignment/server/index.html).

``` 
# create environment named mafft
conda create -n mafft
```

This only creates the mafft enviroment, but it has not yet let you do anything to it. To install programs or use the environment, you must first activate it.
```
# activate conda environment
conda activate mafft
```

Now you should be "inside" the mafft environment (you should see mafft in the parenthesis). You can now install the actual mafft program. Many programs live in specific online places called channels. You can tell conda to look at specific channels with the "-c" flag. In this case, we will use bioconda.

```
# install mafft
conda install -c bioconda mafft
```

A bunch of stuff should be printed at you and you will have to say yes to installing things, but then the program should be installed. Unless you want to immediately use what you installed, you should next deactivate the conda environment (if you do not do this you run the risk of accidentally installing other programs that may not play nicely with your original progam).

```
# deactivate
conda deactivate
```

### Singularity

