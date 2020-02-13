# BGI-HiC-Computational-Analysis
Scripts to analyze BGI HiC data and produce contact maps


Simply download the `BGI HiC computational analysis  (Sandoval-Velasco et al., 2020).ipynb` file and open it in Jupyter Notebook. See https://jupyter.org/install.html for details on installation. Make sure you install the Jupyter Notebook, and not the Jupyter Lab. Installation should not take more than 10-15 minutes on a desktop computer)

This notebook just contains the instructions to go from the `*.fastq` files to the generation of HiC matrices.
The software used is TADBit (Serra et al., 2017), invoked through the command line. 
If you install the Jupyter Notebook bash kernel (more info http://slhogle.github.io/2017/bash_jupyter_notebook/) you can directly run the commands in-situ in the notebook. Alternatively, you can run bash in the Notebook if you add the characters: `%%bash` to the beggining of the each execution cell, so that the interpreter knows that it should use bash as the language to use.

Otherwise, it serves as a bioinformatics protocol to perform your analysis. Just copy the instructions in order to your Terminal, run it, and it will work just fine.



#### References:

Serra F, Baù D, Goodstadt M, Castillo D, Filion GJ, Marti-Renom MA (2017) Automatic analysis and 3D-modelling of Hi-C data using TADbit reveals structural features of the fly chromatin colors. PLoS Comput Biol 13(7): e1005665. https://doi.org/10.1371/journal.pcbi.1005665
