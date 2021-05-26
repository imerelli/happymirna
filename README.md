# HAPPYMIRNA
Happymirna is a tool for the integration of miRNA-target predictions and comparison.

---
### Prerequisites
* Java 1.7 (or higher)

---
### Download and Installation
The software is available at Bitbucket (https://bitbucket.org/bereste/happymirna).

Happymirna is a Java application distributed as JAR file, and it does not require installation.

---
### Execution

Happymirna consists of two applications.

1. Database preparation (should be run only once for each species):
```bash
$ java -jar <happymirna_dir>/prepareRefDB.jar [-o <out_dir>] -s <species_name>
```
where:

    * `out_dir` is the directory where the reference DB will be created
	* `species_name` is the name of the considered species (hg19, mm10, ...)

2. Run predictions and (optionally) comparisons:
```bash
$ java -jar <happymirna_dir>/happymirna.jar -d <DB_dir> -s <species_name> -f <fasta_miRNA_file> [-o <out_dir>] [-l <comparison_list>] [-t <num_threads>]
```

---
### Contacts

* Stefano Beretta
* Ivan Merelli
