# TreeGubbins

A python script for identifying clusters in phylogenetic trees based on a one dimensional scanning statistic on clade branch lengths.

Requirements:

Requires python 2.x and the dendropy python library

Usage: TreeGubbins.py [options]

Options:<br>
  -h, --help,            show this help message and exit<br>
  -t FILE, --tree=FILE,  Input tree file (NOTE: tree must be fully bifurcating)<br>
  -o OUTPUT, --output_prefix=OUTPUT,
                        Output prefix<br>
  -s FLOAT, --significance=FLOAT,
                        Significance cutoff level [default= 0.05]<br>
  -p INT, --permutations=INT,
                        Number of permutations to run to test significance
                        [default= 100]<br>
  -m, --midpoint,        Midpoint root output tree pdf [default= False]<br>
  -l LADDERISE, --ladderise=LADDERISE,
                        ladderise tree (choose from right or left) [default=
                        none]<br>
  -i, --iterative,       Run in iterative mode, which allows nested clusters.
                        Default = do not run iteratively (much faster)<br>

Output:
The csv file produced by TreeGubbins can be viewed along with the tree in Phandango: http://www.phandango.net
