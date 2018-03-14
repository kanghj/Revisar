# Overview #

<p style="text-align: justify;">
Code analyzers such as ErrorProne and FindBugs detect code patterns symptomatic of bugs, performance issues, or bad style. These tools express patterns as quick fixes that detect and rewrite unwanted code patterns. However, it is hard to come up with new quick fixes and decide which ones are useful and frequently appear in real code. We propose to rely on the collective wisdom of programmers and learn quick fixes from revision histories in software repositories. We propose Revisar, a tool for discovering common Java edit patterns in code repositories. Given code repositories and their revision histories, Revisar (i) identifies code edits from revisions, (ii) clusters edits into sets that can be described using an edit pattern, (iii) compiles, when possible, the edit patterns into executable plugins for the Google's ErrorProne tool. The patterns can then be inspected by the designers of code analyzers. We ran Revisar on nine popular GitHub projects, and it discovered 920 edit patterns across projects. We then acted as designers of code analyzers, inspected the most common 381 patterns and classified 32 as quick fixes. To assess the quality of the quick fixes, we performed a survey with 164 programmers from 124 projects, showing the 10 edit patterns that appeared in most projects. Programmers supported 9 (90%) patterns. We submitted 20 pull requests applying our patterns to 9 projects and, at the time of the writing, programmers supported 17 (85%) and accepted 10 of them.
</p>

[Reudismam Rolim](http://www.dsc.ufcg.edu.br/~spg/reudismam/), [Gustavo Soares](https://gustavoasoares.github.io/), [Rohit Gheyi](http://www.dsc.ufcg.edu.br/~rohit/), [Loris D'Antoni](http://pages.cs.wisc.edu/~loris/)

This paper is available on [here](https://arxiv.org/abs/1803.03806).
