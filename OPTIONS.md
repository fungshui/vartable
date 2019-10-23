# VarTable Options

## (Required)
**--input-vcf**		input VCF file

*	Do we need to differentiate between NGS_Mapper VCF (every position) versus lofreq VCF (only variants)?*

**--input-bam**		input BAM file

*	Do we assume BAM index file is in the same directory as BAM or should we include it as an option?

*--input-bai	input BAM index file*

**--input-ref**		input reference FASTA file

*	Assuming we are using a GenBank ref, are we planning to parse annotated data?*

*--accession	input reference fASTA accession number to parse GenBank information*

**--minpercent**	input variant call percentage (at what frequency do we call a nt a variant)

*	Required b/c we cannot assume the level 20%, 5%, 1%... it also prevents a mistaken run by user*

**--minbq**		input minimum base nt quality

*	Required b/c we cannot assume the quality 25%, 30%... it depends on --minpercent*


## (Optional)
**--input-prm**		input primer FASTA file

**--mindepth**		input minimum depth of coverage for each nt base

*	Should we set this automatically to a default of 10? For our usage, 10 does not change*

**--output-name**	input the desired output filename (default format: tsv)

*	Optional b/c I am assuming a generic output name can be given if none is given*

**--output-dir**	input the desired output directory

*	Optional b/c I am assuming VarTable is able to output into current working directory if none is given*

*--output-err	input name of output error file for user troubleshooting or submit the error file for help*

*	Instead of the user gathering all pertinenet run information, error file should contain it for quick help*
