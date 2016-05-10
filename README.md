# README for Calculating Distance Between Alpha Carbons in a PDB File (Distcalc.rmd)

## General

The R piece of code will read a pdb file and find the distance between two selected alpha carbons.

The R tool that accomplishes this task is named distcalc. Distcalc takes 5 required inputs: inputfile, index1, index2, outopts, and outputfile. The indices (index1 and index2) correspond to the alpha carbon of the nth residue. The input inputfile is the name of a corresponding pdb file from which to calculate a distance. The code will run after loading the function from the distcalc.rmd file.

### Input Options for discalc:

1. inputfile - the name of the input file (1a3n.pdb)
2. index1 - integer index of 1st amino acid in sequence to calculate the distance of its alpha C to other (2)
3. index2 - integer index of 2nd amino acid in sequence to calculate the distance of its alpha C to other (9)
4. outops - integer (either 0,1,2) to determine output format
  + 0 : outputs distance in angstroms to console
  + 1 : outputs distance in angstroms to txt output file called output.txt
  + 2 : outputs distance in angstroms to txt output file and amino acid sequence of the protein in the pdb file
5. outputfile - the desired name of the output file ("output.txt")

### Usage

```{r}
distcalc(inputfile = "1a3n.pdb", index1 = 43, index2 = 44, outops = 0, outputfile = "output.txt") 
```
### Other

* [CBB 752 Final Project Website](http://cbb752spring2016.github.io/)
* [Distcalc.py](https://github.com/peter-mm-williams/Python_Distance_Calculation), brought by [Peter](https://github.com/peter-mm-williams)
