# Shifted Hamming Distance

Shifted Hamming Distance (SHD) is an edit-distance based filter that can quickly check whether the
minimum number of edits (including insertions, deletions and substitutions) between two strings is
smaller than a user defined threshold **T** (the number of allowed edits between the two strings).

Testing if two stings differs by a small amount is a prevalent function that is used in many
applications. One of its biggest usage, perhaps, is in DNA or protein mapping, where a short
DNA or protein string is compared against a enormous database, in order to find similar matches. In
such applications, a query string is usually compared against multiple candidates strings in the
database, where the similar matches are reported.

SHD expands the basic Hamming distance computation, which only detects substitutions, into a
full-fledged edit-distance calculator, which counts not only substitutions but insertions and
deletions as well.

The algorithm of SHD is described at: [ H. Xin et al., **Shifted Hamming Distance: A Fast and Accurate SIMD-Friendly Filter to Accelerate Alignment Verification in Read Mapping**, Bioinformatics ](http://bioinformatics.oxfordjournals.org/content/early/2015/01/10/bioinformatics.btu856.abstract)


