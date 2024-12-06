# rust-samtools-viewer

- rust samtools view. 
- given an sam alignment file and a give range of the coordinate from the genome, will produce a colour coded alignment for the reads aligned in that region. 
- Especially important for showing the reads specific to abundance, metabolites, genomic association to phenotypes.
- general note: Incase of Golang and RUST, please see the last commit message and if it says compiled binary then it is completed or else still in development version.
- This feature is not present in samtools. 

![](https://github.com/applicativesystem/rust-samtools-viewer/blob/main/rust-samtools-viewer.png)
- explanation : The first read related to the normal phenotype, the second to the diseased one and the third one to the mutant and so on. 

```
cargo build
```

```
Usage: rust-samtools-viewer <ALIGNMENT_ARG> <GENOME_START> <GENOME_END>

Arguments:
  <ALIGNMENT_ARG>  please provide the path to the alignment file
  <GENOME_START>   please provide the genome capture region start
  <GENOME_END>     please provide the genome capture region end

Options:
  -h, --help     Print help
  -V, --version  Print version
```

- sample view from the sample alignment, choose any number or coordinate from your aligned file. 

```
./target/debug/rust-samtools-viewer ./sample-files/alignreads.sam 200 250

```


Gaurav Sablok
