# An Analysis of ETE Discussion Posts

ETE is my 2-year university program where we routinely discuss problems and solutions around climate change, as well as the social and environmental impacts that climate change has had on the world at large. A way to keep us thinking about issues is through weekly discussion posts, in which we're presented a new or recurring topic (like regenerative agriculture, nuclear energy, sustainable cities, biomimicry, and more) accompanied with a few articles containing stories, facts, or opinions around those topics, and are asked to give our thoughts. This notebook/repo analyzes changes in word count and lexical richness + readability through the first 3 semesters. [Here](https://github.com/zsat/ete-discpost-analysis/blob/main/ete_discpost_analysis.ipynb)'s the notebook for more explanation + discussion, as well as the code (try Chrome if Safari glitches for you).

--- 

## Findings

- We're writing (on avg.) 20% more each semester. Mean words jumped by 100 from ~240 to ~340 across 3 semesters. Median words jumped by ~80 in the same span, about a 36% increase
- Our vocabulary gets better each semester (lexical richness, measured by MTLD) 
- Our sentence/word length (lexical readability) stays relatively the same - perhaps a good thing
- It seems like we're writing with a slightly broader vocabulary, but not making our sentences overly complex, rather we're keeping them accessible to the average reader (which in my opinion is one of the better possible scenarios).

### Looking at word count

- **Mean + median word counts, per semester**
  - Certainly increasing every semester (about a 10-25% increase/sem).
  - Mean is biased up, so I'll use median as measure of centrality.

<img src="imgs/meanmed.png" width="65%">

- **Word count distributions, per semester**
  - We see left-leaning centrality every semester, it appears we tend to like to hit a minimum word count & higher counts become exponentially rarer.
  - Variance in word count increases every semester - are we caring less about how much people before us wrote? Are we enjoying the content more? I can answer the first question with more code, but the second is better asked to students.
  - Most of us didn't have prior coursework with sustainability, so it could be that we're becoming more drawn toward the topics as time goes on (this definitely is the case for me) and thus freely write more.

<img src="imgs/histograms.png" width="90%">

Fun note: our 3-semester progression is almost indistinguishable from a 3-complexity-level progression of writings from children ages 7-16, collected by WeeBit. The histograms below at least shows us that the pattern we see in ETE has also been seen with other people - might provide insight, but as of now I see it as just interesting. \[[Source](http://cs229.stanford.edu/proj2018/report/185.pdf)\]

<img src="imgs/levels_hist.png" width="55%">

---

### Measures of Complexity

- **Lexical Readability**
  - Lexical readability mainly accounts for sentence and word length - tries to quantify how 'hard' or 'easy' a text is to read.  
  - Each metric outputs an American K-12 grade level of readability, so ~13 means a college freshman is easily able to read the texts.
  - Text Standard is the most comprehensive measure out of the 4, so it appears we're not over complicating our texts over our 3 semesters - just staying consistent.

<img src="imgs/readability.png" width="70%">

- **Lexical Richness**
  - Instead of text length, richness tries to measure vocabulary.
  - A common metric is TTR, which is the % of unique words in a text - this of course is biased towards shorter texts.
  - Although TTR goes down every semester, we've seen our text length goes up.
  - A better metric that avoids this bias is MTLD, which we see increases every semester, implying our true vocabulary is improving.

<img src="imgs/richness.png" width="70%">

(Note that the ranges for these metrics aren't the mins/maxes, I just narrowed the window to make them more readable)

---

## Conclusion

It seems like we're writing with a slightly boarder vocabulary, but not making our sentences overly complex, rather we're keeping them accessible to the average reader (which in my opinion is one of the better possible scenarios).
