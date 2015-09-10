---
layout: post
title: The Skeleton in the Closet
---

![headimg]({{ site.baseurl }}/images/IMG_1618.JPG)
After a few [ups](http://www.ecoevoblog.com/2014/10/13/phd-positive-happy-developments/) and [downs](http://www.ecoevoblog.com/2014/10/06/phd-pretty-huge-disaster/), everything you always wanted to know about the effect of missing data on recovering topology using a Total Evidence approach is now [available online (Open Access)](http://www.sciencedirect.com/science/article/pii/S1055790315002547)!

This paper also treats many different questions that people might be interested in (Bayesian vs. ML; how to compare tree topologies; comparing entire distributions, not only their means and variance; and many more!) but I’ll leave it to you to discover it…

Back on track, more than one an a half CPU centuries of calculation ago, [Natalie](http://nhcooper123.github.io/) and myself wanted to build a [Total Evidence tip-dated primates tree](http://www.ecoevoblog.com/2013/03/29/dinosaurs-are-useless-if-they-dont-go-in-trees/). The **Total Evidence method** is the method that allows you to combine both living and fossil species (or actually, read "both molecular and morphological data"''") into the same phylogenies. The **tip-dating method**, is an additional method that uses the age of the tips rather than the age of the nodes for dating such a tree. But I’m not going to talk about that in this post.

At the start of the project, we were both confident about the idea behind it and that primates would be the ideal group for such work since they are so well studied. A study that I described in a [former post](http://www.ecoevoblog.com/2014/01/13/a-brave-new-world-of-monkeying-around-with-trees/) also came out around the same time, encouraging us and comforting us in this project.

However, as you might guess, something went wrong, horribly wrong! For the Total Evidence method, we need molecular data for living species ([check](http://journals.plos.org/plosone/article?id=10.1371/journal.pone.0049521)) morphological data for fossils species ([check](http://www.nature.com/nature/journal/v498/n7452/full/nature12200.html)) and also for living species (che… No, wait)! After looking at the available data, we quickly found out that there was a crucial lack of living taxa with available morphological data (check our preprint to be submitted to Biology Letters putting the actual numbers on the problem). From that problem, rose the idea of actually testing how that would influence our analysis. And funnily enough, this problem become one of the two major parts of my PhD!

Running thorough (and loooooong) simulations, we assessed the impact of missing data on topology when using a Total Evidence method. We looked at three parameters where data would be missing:

* The first one, was obviously the one I introduced above: the **number of living taxa with no available morphological data** (at all!).
* The second one, was the **amount of available data in the fossil record** (because yes, fossils can be a bit patchy).
* And the third one, the **overall amount of morphological characters**.

We then compared the effect of different levels of available data for each parameter individually and and their combination on recovering the correct topology, using both Maximum Likelihood and Bayesian Inference. For the correct topology, we used the tree that had no missing data in our simulations. For each parameter combination, we measured the clades in common between the correct topology and the trees with missing data as well as the placement of wild-card taxa (typically fossils jumping everywhere).

Unsurprisingly, we found that the number of living taxa with no available morphological data was the most important parameter for recovering a good topology. In fact, once you go past 50% living taxa with no morphological data, the two other parameters have no effect at all, even if you have a perfect or a really bad fossil record or many or really few characters. This is kind of intuitive when you think about it because the only way to branch the fossils to living taxa is to use the morphological data. Therefore, if there are no morphological data for the living taxa, the fossils cannot branch with them regardless of the quality of the data. Therefore, in this paper, we argue that to improve our topologies in Total Evidence, we should visit more Natural History museums. And not only the exciting fossil collections but the well curated collections of living species as well!

All the code for this paper is available on [GitHub](https://github.com/TGuillerme/Total_Evidence_Method-Missing_data).

Check out the [latest presentation](http://www.slideshare.net/ThomasGuillerme/total-evidence-phylogenies-the-missing-data-issue) about both papers.

**Paper 1**: Guillerme & Cooper 2015 – E*ffects of missing data on topological inference using a Total Evidence approach* – Molecular Phylogenetic and Evolution ([doi:10.1016/j.ympev.2015.08.023](http://dx.doi.org/10.1016/j.ympev.2015.08.023)).

**Paper 2 (preprint)**:  Guillerme & Cooper 2015 – *Assessment of cladistic data availability for living mammals* – bioRxiv ([doi: http://dx.doi.org/10.1101/022970](http://biorxiv.org/content/early/2015/07/28/022970)).


**Photo credit**: Thomas Guillerme (AMNH collections)

**[Original post](http://www.ecoevoblog.com/2015/09/10/the-skeleton-in-the-closet/)**


