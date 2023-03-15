# cluster density is critcally metic that influence run quality, reads passing filter and total data output. 
It is imporant to mainting optial cluster denisty to maximize total data output while avoid negative effcets of overclustering.

overclustering
==============
### What is Q30
Q = − 10 log10 P <br>
if Phred assigns a Q score of 30 (Q30) to a base, this is equivalent to the probability of an incorrect base call 1 in 1000 times. <br>

1.Lower Q30: overloaded signal intensities, the ratio of base inetensity to background for each base is decreased and results in ambigity during base calling.
decrease in data quality <br>
2.Lower Clusters Passing Filter: the %PF is an indication of signal purity from each cluster. this leads to poor template generation, which then cause a decrase in the & PF metric.<br>
3.Lower dataoutput: reduced yield is a byproduct of lower %PF <br>
4.Inaccurate demuliplexing: index reads ussually have low diveristy by design, which can lead to poor base calling.<br>

Intensity drops and lower Q30
