---
title: Using Bibliography in LaTeX
layout: post
guid: urn:uuid:7b53a277-ae92-4f92-bf04-3066541b6057
tags:
  - LaTeX
  - Dissertation
---

I have to rebuild my bibliography library for my thesis. I try to export citation information from Scopus or Google Scholar, but some of the article titles of outcomes kept the uppercases. In ```biblatex```, they will be handled with sentence cases to fix the APA citation style. Here is the issue comes, the ```biblatex``` cannot identify the special terms like Winsteps or person names which should be kept as uppercases.

If I export the references to Mendeley and then export to a ```bib``` database, the ```title``` field would be marked with an additional ```{}``` which means that the ```biblatex``` should not change the cases within. However, this will be unexpected if there were titles in uppercases. The current solution is export the references in Scopus to ```bib``` database first and then import to Jabref. Also, specific modifications should be made to keep the special words as uppercases and then export to readyly used ```bib``` library. However this approach is very time comsuming if there are lots of modifications should be made.

Seeking help from the substitue function in VIM or program a function in R might be alternative approaches but need to be explored first.
