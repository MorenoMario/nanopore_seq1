cat *fastq.gz > FAT27647_all.fastq.gz
seqkit seq -Q 8 FAT27647_all.fastq > FAT27647_all.filt.Q8.fastq
nohup NanoPlot --fastq FAT27647_all.filt.Q8.fastq --outdir nano_qc_filt --threads 60 --loglength &
