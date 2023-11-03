# benchAMRking
BenchAMRking is an easy-to-operate platform where users can access and explore a range of best-practice tools, workflows and data for the prediction of AMR genes from WGS data. The workflows have been implemented in Galaxy to facilitate easy access and use of AMR gene prediction bioinformatics tools for researchers. BenchAMRking workflows are free with supporting self-learning training material.

## WF1: abritAMR
[doi.org/10.3390/microorganisms10020292](https://doi.org/10.3390/microorganisms10020292)  
abritAMR is available as a galaxy tool. The tool is wrapped in two separate workflows. The first one runs abritAMR starting from assemblies. The second one stars includes `shovill` to assemble the input fastq before running abritAMR.

Workflow: <https://workflowhub.eu/workflows/470>  

## WF2: Sciensano
[doi.org/10.1099/mgen.0.000531](https://doi.org/10.1099/mgen.0.000531)  
The following workflow is available on Sciensano's galaxy instance. The workflow starts from fastq.

To run the workflow, go to [sciensano galaxy](https://galaxy.sciensano.be/root?tool_id=pipeline_stec_1.0).
Upload your data:  
![Screenshot uploading data]()

Change the settings according to your requirements, and execute the workflow:  
![Screenshot execute workflow]()

### Extra
Dataset: 137 STEC isolates - [BioProject PRJNA633966](https://www.ncbi.nlm.nih.gov/sra?linkname=bioproject_sra_all&from_uid=633966)  
Assemblies: [STEC isolate assemblies](https://workflowhub.eu/workflows/407/git/1/download/Assemblies/SKESA_assemblies.tar.gz)  

## WF3: CFIA
!! This workflow has pending changes to the public galaxy instance. !!  
[doi.org/10.3389/fmicb.2020.00549](https://doi.org/10.3389/fmicb.2020.00549)  

The workflow is available [here](https://usegalaxy.eu/workflows/trs_import?trs_server=workflowhub.eu&run_form=true&trs_id=407&trs_version=1) and requires FASTQ files as input.
It also requires the ARGannot and ResFinder databases, which can be downloaded from the following links:  
- [ARGannot_r2.fasta](https://workflowhub.eu/workflows/407/git/1/download/SRST2_databases/ARGannot_r2.fasta)  
- [ResFinder.fasta](https://workflowhub.eu/workflows/407/git/1/download/SRST2_databases/ResFinder.fasta)  

The list of SRA accesssions is available [here](https://workflowhub.eu/workflows/407/git/1/raw/Assemblies/CFIA_SRA_Accessions.txt).
Downloading the samples straight to galaxy is possible by using the [NCBI Accession Download](https://usegalaxy.eu/root?tool_id=toolshed.g2.bx.psu.edu/repos/iuc/ncbi_acc_download/ncbi_acc_download/0.2.8+galaxy0) tool.

Start the workflow with the `Run on usegalaxy.eu` button. Use the dataset collection as input and add both ARGannot and ResFinder as database option for SRST2 before executing the workflow.

Workflow: <https://workflowhub.eu/workflows/407>  
### Extra
Dataset: 137 STEC isolates - [BioProject PRJNA633966](https://www.ncbi.nlm.nih.gov/sra?linkname=bioproject_sra_all&from_uid=633966)  
Assemblies: [STEC isolate assemblies](https://workflowhub.eu/workflows/407/git/1/download/Assemblies/SKESA_assemblies.tar.gz)  

## Staramr - Winnipeg
[doi.org/10.1038/s41467-022-35713-4](https://doi.org/10.1038/s41467-022-35713-4)  

Tool url: <https://bioinf-galactus.erasmusmc.nl/root?tool_id=toolshed.g2.bx.psu.edu/repos/iuc/abritamr/abritamr/1.0.14+galaxy0>  
Dataset: <https://bioinf-galactus.erasmusmc.nl/libraries/folders/F38371f1a2a79cb4e/page/1>  
