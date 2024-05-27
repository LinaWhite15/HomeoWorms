# HomeoWorms <a href=""><img src="https://cdn-icons-png.flaticon.com/512/4681/4681603.png" align="right" width="150" ></a> 
### Analysis Of The Distribution Of Developmental Gene Transcripts In The Intact Body Of The Annelids *Pygospio elegans*, *Platynereis dumerilii* And *Arenicola marina*

This repository is contain the results of a project conducted at the [Bioinformatics Institute](https://bioinf.me/), **aimed** to determine the distribution of transcripts coding developmental genes in three annelid species with different regenerative abilities. 

## General workflow 
- Finding sequences containing homeobox domain[(*blastp*)](https://ftp.ncbi.nlm.nih.gov/blast/executables/LATEST/)
- Annotation of selected sequences functionally and finding possible orthologs [(*eggnog mapper v.2.0.0*)](https://github.com/eggnogdb/eggnog-mapper)
- Conducting an phylogenetic analysis of possible orthologs [(*MAFFT v.7.526*)](https://mafft.cbrc.jp/)
- Performing transcript distribution analysis (*Python*)

## Content description
### Notebooks
- `Phylo.ipynb` - the notebook contains code for constructing phylogenetic trees
- `main.ipynb` - the notebook contains steps of transcript distribution analysis: selection of transcripts according to annotation, code for constructing heatmaps

### Folders
#### data
- `ANTP.fasta`, `all_prot.fasta`, `paired.fasta` - files contain sequences for alignment in fasta format
- `mafft.tree`, `NKL.tre` - phylogenetic trees in Newick format for visualization
- `Amar_maNOG.emapper.annotations`, `Pele_maNOG.emapper.annotations`, `Pdum_maNOG.emapper.annotations` - eggNOG-mapper-annotated transcripts

#### imgs
- `my_tree.png` - visualization of the phylogenetic tree for all analyzed transcripts
- `DiffExp1.png` - hitmap of putative developmental genes found only in *Pygospio elegans*
- `DiffExp2.png` - hitmap of putative developmental genes found in annelids with posterior regeneration
- `DiffExp3.png` - hitmap of putative developmental genes found in all three annelids

## Results
- Possible candidate genes to explain *anterior regeneration* could be **BARX1**, **GSC**
- Possible candidate gene to explain *posterior regenerationn* could be **caudal**

## Authors
- `Belikova Angelina` - BI student
- `Elena Novikova` - supervisor
- `Maxim Nesterenko` - supervisor

If you have any questions or suggestions regarding this work, feel free to adress via email:
Belikova Angelina - kiit8321@gmail.com
