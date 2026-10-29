# 3. Run Orthofinder

[Orthofinder](https://github.com/OrthoFinder/OrthoFinder) is a program that groups genes into gene families (called orthogroups). It can be [installed](https://github.com/treyjscott/computational_tools_for_molecular_biology_fools/tree/main/install_packages) with conda or with singularity.

To run orthofinder, you will need proteome files from relevant species. If you do not know which species are relevant check out [Can I use comparative methods?](https://github.com/treyjscott/computational_tools_for_molecular_biology_fools/tree/main/can_i_do_comp)

Once you have proteomes, you can run orthofinder using something like the .sh script included in this directory.

After running orthofinder, you should check a few things to make sure it ran properly and is giving you useful results. A proper run will result in a directory that looks like Fig 1.
![Fig 1](https://github.com/treyjscott/computational_tools_for_molecular_biology_fools/blob/main/static/img/orthofinder_dir.png)

