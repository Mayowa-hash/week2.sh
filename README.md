# week2.sh
## profile
mkdir output
wget https://www.bioinformatics.babraham.ac.uk/projects/fastqc/fastqc_v0.11.9.zip
unzip fastqc_v0.11.9.zip
cd FastQC
wget 
https://github.com/josoga2/yt-dataset/blob/main/dataset/raw_reads/Chara_R1.fastq.gz?raw=true
wget
https://github.com/josoga2/yt-dataset/blob/main/dataset/raw_reads/Chara_R2.fastq.gz?raw=true
mv Chara_R1.fastq.gz?raw=true Chara_R1.fastq.gz
mv Chara_R2.fastq.gz?raw=true Chara_R2.fastq.gz
fastqc Chara_R1.fastq.gz -o output
fastqc Chara_R2.fastq.gz -o output
    
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Windows-x86.exe
conda activate
sudo apt-get install bzip2
bash Miniconda3-latest-Linux-x86_64.sh

conda install -c bioconda fastp

conda create –name conda-test python=2.7 multiqc
conda activate conda_test
conda install -c bioconda multiqc
multiqc --version

conda install -c bioconda samtools
conda install -c bioconda qualimap
