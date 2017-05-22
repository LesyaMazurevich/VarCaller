# VarCaller

VarCaller is the worlds most lightweight varaiant caller!

It is a wrapper that uses samtools and bcftools to call variants.

Input is processed as one or two reads and is mapped to the reference (a fasta or a genbank file, more support for other file type coming) via BWA mem.  From there variants are called using samtools and bcftools. 

Current dependencies: Python (version 2.7), BioPython, samtools (version 1.4), bcftools (version 1.2), BWA (version 0.7.15)

I recomend using the homebrew package manage to install these depenencies.  This can be done using the following commands:

Note, you may need to sudo some of these commands.  Run as root at your own risk!

# Install Brew:

/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

# Install samtools:

brew install homebrew/science/samtools 

# Install bcftools:

brew install homebrew/science/bcftools

# Install BWA:

brew install bwa

# Install wget

wget http://biopython.org/DIST/biopython-1.69.tar.gz

# Unpack BioPython 

tar -xzvf biopython-1.69.tar.gz 

# Build BioPython

python setup.py build
python setup.py test
sudo python setup.py install
