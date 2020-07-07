# BGI-HiC-Computational-Analysis 
Scripts to analyze BGI HiC data and produce matrices and contact maps, as showed in Sandoval-Velasco *et al.,* (under review) paper titled: *"Hi-C chromosome conformation capture sequencing of avian genomes using the BGISEQ-500 platform"*

### Installation:
Detailed instructions come within the `.ipynb` or `.html` flavours of the protocol `BGI HiC computational analysis  (Sandoval-Velasco et al., 2020)`

### HTML text version:

If the Jupyter Notebook world is not something you are into, it serves as well as a bioinformatics protocol to perform your analysis. Just download the `BGI HiC computational analysis  (Sandoval-Velasco et al., 2020).html` version, open it with any web browser and copy the instructions in order to your Terminal, run it, and it will work just fine.

### Using Jupyter Notebook:

Download the `BGI HiC computational analysis  (Sandoval-Velasco et al., 2020).ipynb` file and open it in Jupyter Notebook. See https://jupyter.org/install.html for details on installation. Make sure you install the Jupyter Notebook, and **NOT** the Jupyter Lab. Installation should not take more than 10-15 minutes on a desktop computer.

This notebook just contains the instructions to go from the `*.fastq` files to the generation of HiC matrices in the paper.
The software used is TADBit (Serra et al., 2017), invoked through the command line. 

If you install the Jupyter Notebook bash kernel (more info http://slhogle.github.io/2017/bash_jupyter_notebook/) you can directly run the commands in-situ in the notebook. Alternatively, you can run bash within the Jupyter Notebook default Python kernel if you add the characters: `%%bash` to the beggining of the each execution cell, so that the interpreter knows that it should use bash, and not Python, as the interpreter to use.

### **NOTE 1:** Regarding supplementary figures S2 and S3 on the paper:
Follow the protocol with TADbit, and once the mapping is done, check your working directory for the QC plots of the HiC digestion and histograms of the fragment size distribution. These two kinds of plots are generated always by TADbit as default after the mapping process.

### **NOTE 2:** Regarding tables 1 and 2 in the paper:
You can get the numbers for the statistics we use if you run the `tadbit describe` command. It will display a record of everything that has been run on that folder. Also, it shows some statistics regarding mapping, filters and others.

*TABLE 1:*

Check above **section 1.3** for the `tadbit describe` command on how to get the stats for the numbers in table 1.
Data for the fields in the table named `% Digested sites (out of 100K reads)` and `% Reads with ligation site (out of 100K reads)` was obtained from the QC plot we obtain after the mapping.

*TABLE 2:*

Data from this table was directly imported from the filters section after running the the `tadbit describe` command. 

See the main protocol `BGI HiC computational analysis  (Sandoval-Velasco et al., 2020).ipynb` for further details.

#### References:

Serra F, Baù D, Goodstadt M, Castillo D, Filion GJ, Marti-Renom MA (2017) Automatic analysis and 3D-modelling of Hi-C data using TADbit reveals structural features of the fly chromatin colors. PLoS Comput Biol 13(7): e1005665. https://doi.org/10.1371/journal.pcbi.1005665
