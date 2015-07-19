---
layout: post
title: Hopsolete Trees
---

![headimg]({{ site.baseurl }}/images/Beer_bottles-300x205.jpg)
One of the most unusual benefits of being in Ireland from a Southern French PhD student’s perspective is not so much the rain and the pronounced taste for culinary oddities ([some weird](http://j8.ly/popular-irish-chinese-dish-3-in-1-fried-rice), [some excellent](http://en.wikipedia.org/wiki/Breakfast_roll)) but the awesome trend towards a new age of craft beers (and I’m not mentioning the pillar of [Irish pub culture](http://en.wikipedia.org/wiki/Guinness)).

Looking at the increasing beer richness available in any decent pub/off-licence, I was inspired to combine two of my passions: beer-related stuff and phylogeny-related stuff. Despite an honourable attempt by [J.L. Brown](http://www.jasonleebrown.org/jasonleebrown.org/beerlogeny.html), I would like to discuss the three reasons why it’s imphopsible to build a true beer phylogeny. Admittedly one of the main reasons for this impossibility is the side effect of drinking any sugar rich (at least originally) drink that has been infected by [*Saccharomyces cerevisiae*](http://en.wikipedia.org/wiki/Saccharomyces_cerevisiae)... But there are also three more theoretical reasons.

**To build phylogenies, you need data.**

Despite the fact that the data collection part of such a study could be great (doing your fieldwork in a pub, isn’t that cool?), I doubt the data base would actually be big enough to infer any well supported phylogenetic trees. Think about a matrix with only one character (let’s say presence or absence of bones) and with 4 species (a fly, a tuna, a pigeon and a walrus); you won’t be able to resolve the tree past the first node. Theoretically one needs at least a number of characters equal to the number of taxa (- 2 because you can cheat by ignoring the first and the last node).

Let’s see what our data matrix looks like for beers: there are approximately [180 different beer styles](http://en.wikipedia.org/wiki/Beer_style) out there so we need at least 178 characters to classify them. Even if some characters come readily to your mind (ABV – alcool! –, colour, ingredients, taste), I’ll bet you cannot find more than 10 of them.

**To build phylogenies, you need models.**

When building a phylogeny, it is important to remember that the true questions we are asking our software are something like: (1) which tree involves the minimum number of changes or (2) which is the most likely tree regarding my data?

The first question is the cladistics approach; using an optimal criterion parameter (usually parsimony) when you’re building your tree. It states that the best tree will be the one implying the least number of changes for grouping the tips together. The second question is the probabilistic approach, which is based on fitting a model of character evolution that will be the best fit for the data.

Going back to our brews, the question we want to ask the software will mainly depend on the assumptions we have. A cladistic approach such as the one that [Brown](http://www.jasonleebrown.org/jasonleebrown.org/beerlogeny.html) used works as long as we have sampled enough characters back in the pub. However, unless each clade of beers has a clear pattern (e.g. only the stouts have an ABV between 4.5° and 5°) we are likely to suffer from the well-known [Long Branch Attraction](http://en.wikipedia.org/wiki/Long_branch_attraction) artifact in some parts of the tree.

So can we use the probabilistic method instead? Again, as long as we have enough data, this method is possible but will it give an accurate result? Well, that depends on your model of character evolution. Since we cannot use the classic [DNA evolution models](http://en.wikipedia.org/wiki/Models_of_DNA_evolution), we will have to build our own evolutionary model implying that we have a reasonably guessable probability of going from one state to another for any character (e.g. the probability of moving along the [Standard Reference Method](http://en.wikipedia.org/wiki/Standard_Reference_Method) color scale).

By the way, Spencer and Wilberg ([Cladistics – 2013](http://onlinelibrary.wiley.com/doi/10.1111/cla.12018/full)) tested the actual evolutionary meaning of the two methods (although, they were fairly biased in favour of one of the two approaches).

**To build phylogenies, you need... evolution.**

A last point to this whole problem is that trying to reconstruct a realistic scenario of a clade’s evolution (i.e. a phylogeny) implies that the mechanism underlying the whole process is mainly descent with modification (but this is not exclusively necessary e.g. [evolutionary linguistics](http://en.wikipedia.org/wiki/Evolutionary_linguistics) or [horizontal transfer](http://en.wikipedia.org/wiki/Horizontal_gene_transfer) – see my [previous blog post](http://www.ecoevoblog.com/2013/01/11/hey-tree-of-life-hows-it-growing/) or some more serious (awesome) views [here](http://www.pnas.org/content/96/7/3801), [here](http://www.nature.com/nature/journal/v431/n7005/full/nature02848.html) or [here](http://mbe.oxfordjournals.org/content/29/6/1545)).

Regarding these three points, I must reluctantly abandon the idea of doing any proper beer phylogeny since it seems that a beer-types classification would look more like a massive network than a straightforward textbook example of a phylogenetic tree... To end with a more positive and less phylo-nerd point, these messy relationships between each type of beer allow us to enjoy creative, new craft beers such as [Irish Pale Ales](http://en.wikipedia.org/wiki/Galway_Hooker_%28beer%29) or [Oyster Stouts](http://en.wikipedia.org/wiki/Porterhouse_Brewery) which are more than the sum of every element composing their name.

And for those that just don’t care, I’ll leave you with this excellent [post by Barley McHops](http://aleheads.com/2010/11/30/in-defense-of-beer-styles/) from the [aleheads](http://aleheads.com/2010/11/30/in-defense-of-beer-styles/) blog while I’m going to continue my sampling... Just in case...

**Photo credit**: wikimedia commons

**[Original post](http://www.ecoevoblog.com/2014/04/11/hopsolete-trees/)**
