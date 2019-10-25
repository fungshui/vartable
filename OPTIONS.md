## VarTable Options



Usage
---------

    $ vartable_report --input-vcf [../filename.vcf] --type [basecaller] \
		--input-bam [../filename.bam] --input-ref [../filename.fasta] \
		--minpercent [20] --minbq [25] --mindepth [10] \
		--output-err [filename.err] --input-prm [../filename.fasta] \
		--output-name [filename.tsv] --input-region [10 200] \
		--stats

## (Required)
**--input-vcf**		input VCF file

**--type**		input flag (base_caller | lofreq), this differentiates b/t a VCF with all positions and VCF with only variant positions

**--input-bam**		input BAM file

**--input-ref**		input reference FASTA file or GenBank, gb extension file (this will parse for annotated information)

**--minpercent**	input variant call percentage, for example 20%, 5% or 1%

**--minbq**		input minimum base nt quality, for example 25% or 30%

**--mindepth**		input minimum depth of coverage for each nt base, for example 10

**--output-err**	input name of output file for user troubleshooting or submit the error file for help

## (Optional)
**--input-prm**		input primer FASTA file

**--output-name**	input the desired output filename (default format: tsv)

**--input-region**	input start and end positions; variant table will isolate variants within that region

**--stats**		outputs a file containing genome statistics
