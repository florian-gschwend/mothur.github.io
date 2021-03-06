---
title: 'mothur v.1.17.0'
redirect_from: '/wiki/Mothur_v.1.17.0.html'
---
February may be the shortest month of the year, but that doesn't keep
us from releasing two updates in the month! We are happy to announce the
release of [mothur v.1.17.0](/wiki/mothur_v.1.17.0). We are excited
about the mothur workshop in Detroit next week and are already planning
for the next workshop towards the end of April, if you are interested in
learning more, please let me know.

This release has several new commands for performing hypothesis testing
to compare groups of samples including commands for performing the [
analysis of molecular variance](/wiki/amova), [ test of homogeneity
of variance](/wiki/homova), [ analysis of
similarity](/wiki/anosim), and [ Mantel's
test](/wiki/mantel). We previously discussed using [AMOVA and
HOMOVA with DNA sequences](https://www.ncbi.nlm.nih.gov/pubmed/18239608)
and are finally bringing that functionality to mothur for comparing
groups of samples.

Another important facet of this release relates to fixing a number of
critical bugs in how we were calculating the unifrac distances. If you
have previously used mothur's calculation of these values, please
re-calculate them with the latest version. We are unsure how significant
these bugs were to to people's analyses. Needless to say, we apologize
for any problems this may cause people and are very grateful to those
that have brought these problems to our attention. If you know of anyone
using mothur that isn't receiving these emails, please spread the word.

Thanks to all of you that have completed our survey. If you haven't
completed it yet, there is still time\...

## New commands

-   [amova](/wiki/amova) - analysis of molecular variance
-   [homova](/wiki/homova) - test the homogeneity of variance
-   [anosim](/wiki/anosim) - analysis of similarity
-   [mantel](/wiki/mantel) - Mantel's test of correlation between
    matrices
-   [make.fastq](/wiki/make.fastq) - make your own fastq files

## Feature updates

-   [chimera.slayer](/wiki/chimera.slayer) - added split parameter
-   [unifrac.weighted](/wiki/unifrac.weighted) and
    [unifrac.unweighted](/wiki/unifrac.unweighted) - added the root
    parameter

## Bug fixes

-   Catchall command not finding files -
    [https://forum.mothur.org/viewtopic.php?f=3&t=1114](https://forum.mothur.org/viewtopic.php?f=3&t=1114)
-   [sub.sample](/wiki/sub.sample) command that caused mothur to
    stall if size was close to total number of sequences in file.
-   unifrac commands - significance scores differing between multiple
    processors or one processors if the number of comparisons was less
    than the number of processors used.
-   unifrac commands that occurred if trees were unrooted.

## Other stuff

-   added \[error\] flag when a command aborts
