# BLAST+
[BLAST+](https://blast.ncbi.nlm.nih.gov/Blast.cgi?PAGE_TYPE=BlastDocs&DOC_TYPE=Download) is a suite of command-line tools to run BLAST.

This project encapsulated BLAST+ into a docker container.

## Usage
```usage
docker run \
    -v data_dir_path:/data \
    -v blast_db_dir_path:/db \
    yookuda/blast_plus \
    blastn \
        -db /db/blast_db \
        -query /data/input_file \
        -out /data/output_file
```
