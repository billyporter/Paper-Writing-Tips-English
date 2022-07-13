<p align="center">
<h1 align="center"> <img src="./pics/icon/ai.png" width="30" /> Paper Writing Tips</h1>
</p>
<p align="center">
  	<a href="https://img.shields.io/badge/version-v0.1.0-blue">
      <img alt="version" src="https://img.shields.io/badge/version-v0.1.0-blue?color=FF8000?color=009922" />
    </a>
  <a >
       <img alt="Status-building" src="https://img.shields.io/badge/Status-building-blue" />
  	</a>
  <a >
       <img alt="PRs-Welcome" src="https://img.shields.io/badge/PRs-Welcome-red" />
  	</a>
   	<a href="https://github.com/MLNLP-World/Paper_Writing_Tips/stargazers">
       <img alt="stars" src="https://img.shields.io/github/stars/MLNLP-World/Paper_Writing_Tips" />
  	</a>
  	<a href="https://github.com/MLNLP-World/Paper_Writing_Tips/network/members">
       <img alt="FORK" src="https://img.shields.io/github/forks/MLNLP-World/Paper_Writing_Tips?color=FF8000" />
  	</a>
    <a href="https://github.com/MLNLP-World/Paper_Writing_Tips/issues">
      <img alt="Issues" src="https://img.shields.io/github/issues/MLNLP-World/Paper_Writing_Tips?color=0088ff"/>
    </a>
    <br />
</p>

<div align="center">
<p align="center">
  <a href="#项目动机">Project motivation</a>/
  <a href="#写前必看">Must see before writing</a>/
  <a href="#%E7%BB%88%E7%A8%BF%E5%BF%85%E6%9F%A5%E6%8A%95%E7%A8%BF%E5%89%8D%E4%B8%80%E5%91%A8%E4%B8%80%E5%A4%A9">Final draft must be checked</a>/
  <a href="#百家之言">The words of a hundred</a>/
  <a href="#组织者列表">list of organizers</a>/
  <a href="#贡献者列表">Contributor list</a>
</p>
</div>

## <img src="./pics/icon/motivation.png" width="25" />Project motivation

Many beginner students often make some common small mistakes when submitting manuscripts. In order to save everyone's time and help everyone to locate some small problems as soon as possible. This project summarizes our own experience in the submission process and the submission experience of some teachers and students around us. I hope it can be helpful to everyone. Due to our limited level, if there are any omissions, please forgive me. thank you all.

>Features of this project：
>
>1. **MUST READ BEFORE WRITING**: Contains some common mistakes, each with examples for a quick overview before you start writing your paper.
>2.**The final manuscript must be checked**: contains some examples, which is convenient to quickly locate whether there are errors in your paper.
>3. **Words of a Hundred Schools**: Some writing resources published on the Internet (not complete, welcome to add) have been compiled to facilitate systematic study.



### Disclaimer

All tips listed in this project are **for reference only** and are not guaranteed to be correct. This paper mainly focuses on the papers of the top conference, and the writing of the papers is subject to the actual needs. Familiarity with writing techniques may lead to writing without obvious blunders, and a good essay requires constant polishing.
All content only comes from the author's personal experience, Internet data, the relevant accumulation of the author's team's daily scientific research work, and the words and deeds of the big men around the author's team. If you have any questions, please submit Issue or PR. In addition, the badges used in this project are from the Internet. If you infringe the copyright of your pictures, please contact us to delete them, thank you.

### Contributions welcome

Paper Writing Tips is currently an ongoing project, if omissions are inevitable, any PR and issue discussions are welcome.

### explain

In the following, the content marked "Attention" is the suggested item that the organizer considers to be (more) obviously controversial.

## <img src="./pics/icon/intro.png" width="25" />Must see before writing

### formula symbol

#### 1. Scalar symbols are represented by lowercase Latin letters

* Important: To avoid confusing the letter l with the number 1, the letter l can be replaced with \ell.

![pics_1](pics/1.png)

#### 2. Use \boldsymbol(Attention) for structured values

* Key Point: Structured values ​​such as sentence sequences, trees, graphs, etc.

![pics_2](pics/2.png)

#### 3. The set of \boldsymbols is available with \mathcal (Attention)

![pics_3](pics/3.png)

#### 4. The vector value is lowercase and bold, the matrix is ​​uppercase and bolder

* Important: Use \mathbf for Latin letters and \boldsymbol for Greek letters

![pics_4](pics/4.png)

#### 5. Use \mathbb for number fields, expectations, etc.

![pics_5](pics/5.png)

#### 6. Keep elements corresponding to the symbols of the set

![pics_6](pics/6.png)

#### 7. Write in a formal style and avoid abbreviations

* don't split up and write do nots
* Possessive 's are converted to of

![pics_7](pics/7.png)

#### 8. Latin Idioms

- e.g., means for example,
- i.e., means that is,
- et al. means and others of the same kind,
- etc. means and others, not used to enumerate people
  - et al. or etc. at the end of a sentence without adding an extra period

![8.png](pics/8.png)

#### 9. English quotation marks

The key positions are as shown, using `` and '' to represent left and right quotation marks respectively, not other symbols or any Chinese quotation marks

![9.png](pics/9.png)

#### 10. Non-breaking space "~"

Use ~ for non-breaking spaces, which do not cause unexpected newlines, eg: ' for left and right quotes respectively, not other symbols or any Chinese quotes.：

```latex
Figure~\ref{} shows the model performance.
Table~\ref{} shows dataset details.
We use BERT~\cite{bert} model.
Section~\ref{} concludes this paper.
```

![10.png](pics/10.png)

#### 11. URL linnk

To use the \url{} command, you need to import the package:

```latex
 \usepackage{hyperref}
```

![11.png](pics/11.png)

#### 12. Quotes only mean so-called, not citation (Attention)

Quoted expressions consider italic \textit{} instead of quotation marks.

![12.png](pics/12.png)

#### 13. Non-single-letter variable names

Variables or symbols with more than one letter such as softmax, proj, enc, etc. in the formula, use the text font, that is, use the \textrm or \textit command.

![13.png](pics/13.png)

#### 14. Using function commands

Many functions and symbols have ready-made commands, such as: \arg{}, \max{}, \sin{}, \tanh{}, \inf, \det{}, \exp{}.

![14.png](pics/14.png)

#### 15. Parentheses in formulas should be marked by \left, \right

![15](pics/15.jpeg)

- Such as \left(\right), \left{\right}, \left<\right>, \left|\right|, etc.

- The division in parentheses is achieved by \middle.

- The latex code is as follows:

    ```Latex
  \begin{gather}
     \bold{s} = \left(\sum_{i=0}^{N-1}{\alpha_{i} \bold{h}_i}\right) + \bold{h}_N\\
     \bold{s} = (\sum_{i=0}^{N-1}{\alpha_{i} \bold{h}_i}) + \bold{h}_N \\
  \end{gather}
  
  \begin{gather}
     \left\{ x \middle| x\ne\frac{1}{2}\right\} \\ 
     \{ x | x\ne\frac{1}{2}\}
  \end{gather}
  ```

#### 16. Use align to represent a set of formulas, with equal signs aligned.

![16](pics/16.jpeg)

- Use align to represent a set of formulas, with equal signs aligned.

- The latex code is as follows:

    ```Latex
  \begin{gather}
     E = m c^2 \\
     C = B \log_2\left(1+\frac{S}{N}\right)
  \end{gather}
  
  \begin{align}
     E &= m c^2 \\
     C &= B \log_2\left(1+\frac{S}{N}\right)
  \end{align}
  ```

#### 17. Only add numbers to the formula of the refer (Attention)

![17](pics/17.jpeg)

- Recommendation: Only add numbers to refer formulas, and \nonumber to number them.

- The latex code is as follows:

    ```Latex
  \begin{equation}
     E = m c^2 
  \end{equation}
  
  \begin{equation}
     E = m c^2 \nonumber
  \end{equation}
  ```

### table image

#### 18. Use Booktabs to draw better-looking tables

![18](pics/18.jpeg)

- When drawing tables, use \usepackage{booktabs} to draw nice dividers with the help of \toprule, \bottomrule, \midrule, \cmidrule commands.

- The latex code is as follows:

    ```Latex
  % Example of a table with booktabs from https://nhigham.com/2019/11/19/better-latex-tables-with-booktabs/.
  % First version of table.
  \begin{table}[htbp]
     \centering
     \begin{tabular}{|l|c|c|c|c|c|l|}
        \hline
        & \multicolumn{3}{c|}{E} & \multicolumn{3}{c|}{F}\\
        \hline
                    & $mv$  & Rel.~err & Time    & $mv$  & Rel.~err & Time   \\\hline
        A    & 11034 & 1.3e-7 & 3.9 & 15846 & 2.7e-11 & 5.6 \\
        B & 21952 & 1.3e-7 & 6.2 & 31516 & 2.7e-11 & 8.8 \\
        C & 15883 & 5.2e-8 & 7.1 & 32023 & 1.1e-11 & 1.4 \\
        D  & 11180 & 8.0e-9 & 4.3 & 17348 & 1.5e-11 & 6.6 \\
        \hline
     \end{tabular}
     \caption{Without booktabs.}
     \label{tab:without-booktabs}
  \end{table}
  
  % Second version of table, with booktabs.
  \begin{table}[htbp]
     \centering
     \begin{tabular}{lcccccl}\toprule
        & \multicolumn{3}{c}{E} & \multicolumn{3}{c}{F}
        \\\cmidrule(lr){2-4}\cmidrule(lr){5-7}
                 & $mv$  & Rel.~err & Time    & $mv$  & Rel.~err & Time\\\midrule
        A    & 11034 & 1.3e-7 & 3.9 & 15846 & 2.7e-11 & 5.6 \\
        B & 21952 & 1.3e-7 & 6.2 & 31516 & 2.7e-11 & 8.8 \\
        C & 15883 & 5.2e-8 & 7.1 & 32023 & 1.1e-11 & 1.4\\
        D  & 11180 & 8.0e-9 & 4.3 & 17348 & 1.5e-11 & 6.6 
        \\\bottomrule
     \end{tabular}
     \caption{With booktabs.}
     \label{tab:with-booktabs}
  \end{table}
  ```

#### 19. References to Chapters, Tables, Figures

-   After chapters, tables, and pictures are defined with \label{...}, they are automatically referenced and jumped through \ref{...}.
-   References to subfigures or subtables can be represented using Figure~\ref{fig:figure}(a).

#### 20. Do not repeat the Caption in the chart in the text

![20](pics/20.jpeg)

- Caption is used to write "What is this table?".
- The body is used to write "what does this table say".

#### 21. "Three-line table" suggestion: try not to draw vertical lines (Attention)

![22.jpg](pics/22.jpg)

#### 22. table resizing

- use \centering Centered；use\small，\scriptsize，\footnotesize，\tiny Adjust font size
- use\setlength{\tabcolsep}{8pt} Adjust column spacing
- use p{2cm} Fixed column width
- use\multirow，\multicolumn Merge Cells

![23.jpg](pics/23.jpg)

#### 23. Vector Graphics: Images should use vector graphics (e.g. in PDF format)

- Use Adobe illustrator, OmniGraffle and other software to draw and save as vector graphics
- useMatplotlib save after drawing: plt.savefig('draw.pdf')
- Drawing directly with pgfplots in LaTeX

![24.jpg](pics/24.jpg)

#### 24. The image font size is between the text font and the caption

- It is recommended to keep the font size in the picture consistent

![25.jpg](pics/25.jpg)

#### 25. The font size of the text description in the pictures in the paper should be the same as the text size of the main text

- The font size of the text in the picture should not be too large

![new_25.jpg](pics/update1_pic_25.png)

#### 26. Graphic design should be suitable for black and white printing

- Friendly to black and white printing: Don't use color as the only feature to refer to the lines in the illustration, use solid/dotted lines, light/dark, different line shapes, etc.

![26.jpg](pics/26.jpg)

#### 27. Keep the picture style simple and beautiful

- Don't use too many colors, avoid too bright colors
- Use concise diagrams and minimize textual descriptions (except examples)
- The same function module uses a unified format
- Arrows should go in the same direction

![27.jpg](pics/27.jpg)

### word choice

#### 28. Pay attention to the part of speech of the hyphen

* 一In general hyphens, the last一A word is a noun, and together it is an adjective part of speech；

![pic_29](pics/pic_29_1.jpeg)

* at last一A word is a verb, and together it is a verb part of speech.

![pic_29](pics/pic_29_2.jpeg)

#### 29. part of speech error

* **First**,  Secondly，both adverbs
* training， **test**，validation，both nouns 

![pic_30](pics/pic_30.jpeg)

#### 30. Abbreviations are customary

* In line with the habit, try to be consistent with the proposer CNN, LSTM, FEVER, ConceptNet, SQuAD, BiDAF, FEVER score, Wikipedia.
* When it first appears, the full name comes first, followed by the abbreviation; or the abbreviation comes first, followed by the citation for annotation。graph attention network (GAT)，pre-trained language model (PLM)；BERT~\citep{BERT}。
* Domain names, task names, indicators, etc. generally do not need to be capitalized, such as natural language processing, question answering, accuracy, macro-F1 score.

![pic_31](pics/pic_31.jpeg)

#### 31. Pay attention to singular and plural

* Especially irregular singular and plural nouns and uncountable nouns.

![pic_32](pics/pic_32.jpeg)

#### 32. a/an follow the vowels

![pic_33](pics/pic_33.jpeg)

#### 33. the usage of

* Notice：一Countable nouns generally do not appear independently (without an article) in the singular, either by adding the specific or by adding the plural to refer generally.

![pic_34](pics/pic_34.jpeg)

#### 34. Tense: Mainly in the simple present tense (Attention)

![pic_35](pics/pic_35.jpeg)

#### 35. Avoid absolute statements。

- replace obvious with straightforward
- Replace always with generally, usually, often
- Use rare instead of never
- Use alleviate, relieve to replace avoid, eliminate

![36.jpg](pics/36.jpg)

#### 36. Avoid vague expressions, such as: meaning, semantic, better, etc.

![37.jpg](pics/37.jpg)

Taking better as an example, that is, when it means that a thing is better, it cannot just be said that it is better, but corresponding explanations and reasons need to be given.

### Sentence expression

#### 37. Avoid excessive use of pronouns: it, they, etc. Model name abbreviations are not too long and clearer.

![38.jpg](pics/38.jpg)

#### 38. Avoid over-labeling, such as when talking about good results.

Where exactly did the proposed method improve and what led to this result?

![39.jpg](pics/39.jpg)

#### 39. Say one thing in a word. Use simple sentences as much as possible and avoid long compound sentences.

![40.jpg](pics/40.jpg)

#### 40. Observation/discovery? Suppose? method? Effect? Don't mix things up.

![41.jpg](pics/41.jpg)

### Paragraph layout

#### 41. When the number of words in a line does not exceed 1/4, it is recommended to delete or increase the number of words. (Attention)
- Optional: try adding `\looseness=-1` at the end of the paragraph, sometimes you can "squeeze" individual words in the last line without deleting the last line.

![pic_42](pics/pic_42.png)

### references

#### 42. Reference citation needs to check whether it is a component in the sentence

* Important: Citations use \citep{}, as an interjection; or \citet{}, as the main components of a sentence such as subject, object, etc.

![pic_43](pics/pic_43.png)

#### 43. Whenever possible, cite the published version rather than the arXiv version。

* will appear more formal

![pic_44](pics/pic_44.png)

#### 44. Citations should be formatted as consistently as possible

* Such as the abbreviation of the conference name, whether to include the time and place of the conference, etc. Whether all the reference formats are consistent

![pic_45](pics/pic_45.png)

## <img src="./pics/icon/resource.png" width="25" />Final manuscript must be checked - one week before submission, one day

### About the Writing Habits of English for Science and Technology

#### 1.  You can refer to spell-checking software to check the text for language errors or irregular expressions.

* E.g [grammarly](https://app.grammarly.com), [writefull](https://www.writefull.com/).

#### 2. Don't use abbreviations like didn't can't don't isn't aren't Don't use an apostrophe for abbreviations at any time. For the possessive, don't use it at all, if you have to express a similar meaning, use the phrase of. For quotation marks, try to avoid them.

#### 3.  Use abbreviations (such as model name, definition, etc.), which need to be defined in the most initial position used.

#### 4.  The case of the model name should be consistent, such as BERT, ELECTRA, and avoid mixed use of Bert, Electra, and electra.

#### 5.  Example sentences, examples consider using italics

#### 6.  \begin\item改成正常段落可以使页面更紧凑（然后在每段前手工加打黑点$\bullet$），浪费过多空间有被怀疑灌水之嫌

#### 7.  Changing \begin\item to a normal paragraph can make the page more compact (and then manually add a black dot $\bullet$ before each paragraph), wasting too much space may be suspected of watering

#### 8.  The difference between A and an is the pronunciation: an LSTM cell, an F/H/L/M/N/S/X, a U.

#### 9.  The capitalization style of the title at all levels of the article is consistent, such as the capitalization of the first letter of a phrase or the first letter of a word

#### 10. Use babel to achieve the effect of word breaking by phonetic syllables (hyphenation patterns), ie `\usepackage[english]{babel}`

### About pictures：

#### 11.  The font inside the image should be uniform and the same size as the text of the text.

#### 12.  Try not to have blank space on both sides of the entire image, keep it compact.

#### 13.  Images are usually at the top or middle of each page, not the bottom。

#### 14. The colors of the same type of modules should be kept in the same color system as much as possible, and each type of unit should be filled with the same color or used as a border。

#### 15.  In the same color system, if a module is darker and brighter, it means that this module is more important. If you don't want to express more important and more core, please maintain a balanced color distribution between each module, for example, the gray value should be as consistent as possible.

#### 16. Do not use too many colors, preferably no more than six colors.

#### 17.  Pictures use vector graphics.

#### 18.  The original intention of figure is to provide a more intuitive, clearer and more concise expression than text. Reasonable drawing elements should be used as much as possible, rather than a large number of text marks. Figure elements, specifications are done with the smallest set, the most uniform, consistent settings, generally not ugly。

#### 19.  Details to line type and color matching: first, keep it uniform (low descriptive complexity), second, with a meaning, category of graphic elements should be similar, the same line shape, color matching (cognitive intuition)。

#### 20.  The directions of the arrows should be kept in the same direction as much as possible to avoid turning back and forth. Avoid isolated components (without any source or destination arrows) in flowcharts.

### About Citations：

#### 21.  Selection of reference marks：

* Quoted out of text（parent），use \cite。

* quoted in text（within text）

  * ACL/NAACL/EMNLP Template use \citet{...}；
  * COLING templates use \newcite{...};
  * AAAI/IJCAI templates use \citeauthor{...} \shortcite{...};
  * IEEE template: \citeauthor{...}~(\citeyear{...})

  Effect：(Zhang et al. 2020) vs. Zhang et al. (2020)

#### 22.  If space is tight, use the abbreviation of the conference journal name in the citation.

* tool for reference [SimBiber](https://github.com/MLNLP-World/SimBiber)

#### 23.  Bib management pays attention to keeping the full name and abbreviation of the conference/journal name consistent, checking the year, volume number, page number, etc., and do not rely solely on the information provided by scholar (there may be missing or confusing formats).

* tool for reference [Rebiber](https://github.com/yuchenlin/rebiber)

#### 24.  After chapters, tables, and pictures are defined with \label, they can be automatically referenced and jumped through \ref.

#### 25.  Leave a space between the citation and the text, not next to the text letter.

#### 26.  Do not repeatedly cite different versions of the same paper, such as arXiv and formal conference papers.

### About formulas：

#### 27.  A formula is part of a sentence. So commas and periods can be added inside formulas (especially on multiple lines).

#### 28. For the text after the formula, if it forms a complete sentence with the formula, the first letter does not need to be capitalized, and it is immediately after the formula; if a new sentence or paragraph is started, a new line should be added after the end character \end of the formula, and the first letter of the sentence should be added. Capitalize letters to start a new sentence.

### Precautions before submitting：

#### 29.  Check articles for anonymity and cannot contain personal and institutional information。

#### 30. Check for overpage (at the last moment, be careful not to arbitrarily change the size of the chart)

#### 31.  Check that the title and abstract correspond to the information in the input box of the submission system。

#### 32.  Check the submitted data and code. It cannot contain personal and institutional information. In particular, some hard coded models or data paths in the code need to be disposed of. In addition, you need to pay attention to hidden folders (such as .git）

#### 33.  Overleaf may be slow to access before some conference submissions, please pay attention to LaTex backup

#### 34.  The historical version of the paper can be numbered with time to avoid submitting a non-final version

#### 35.  It is best to submit a version of the paper and appendices one day before the deadline to prevent the server from crashing when the manuscript is due.

#### 36.  After submitting the manuscript, you still need to pay attention to the conference official website and registered mailbox, and receive the news of the possible extension of the conference deadline in time.

##  <img src="./pics/icon/catalogue.png" width="25" />The words of a hundred

●   [清华大学刘洋老师的CWMT-2014报告：机器翻译学术论⽂文写作⽅方法和技巧](http://nlp.csai.tsinghua.edu.cn/~ly/talks/cwmt14_tut.pdf)

●   [复旦大学邱锡鹏老师的CCL-2018报告：如何端到端地写科研论文？](https://xpqiu.github.io/slides/20181019-PaperWriting.pdf)

●   [清华大学刘知远老师：如何写一篇合格的NLP论文 ](https://zhuanlan.zhihu.com/p/58752815)

●   [中国人民大学赵鑫老师：如何以初学者的身份写好一篇国际学术论文](https://zhuanlan.zhihu.com/p/136005095)

●   [哈尔滨工业大学车万翔老师：如何做一个精彩的学术报告](http://www.cips-cl.org/static/CCL2019/downloads/stuPPT/01.pdf)

●   [香港中文大学（深圳）陈冠英老师整理的写作建议](https://github.com/guanyingc/latex_paper_writing_tips) || [& Rebuttal Template ](https://github.com/guanyingc/cv_rebuttal_template)

●   [哥伦比亚大学 Henning Schulzrinne 老师：Tips and Resources for Writing Computer Science Papers](http://www.cs.columbia.edu/~hgs/etc/writing.html)

●   [哈佛大学 Whitesides 老师：从写提纲的角度切入讲解如何撰写学术论文](https://onlinelibrary.wiley.com/doi/pdf/10.1002/adma.200400767)

●   [卡耐基梅隆大学 Graham Neubig 老师：How to Read/Write an International Conference Paper](http://www.phontron.com/slides/neubig15paperwriting.pdf) & [Paper style guide](http://phontron.com/paper-guide.php)

●   [MSR研究员Simon Peyton Jones老师：How to Write a Great Research Paper](http://research.microsoft.com/en-us/um/people/simonpj/papers/giving-a-talk/writing-a-paper-slides.pdf)

●   [MSRA研究员王晋东：用LaTex写论文经验分享](https://mp.weixin.qq.com/s/XshMg6Qb8ArLNA75ImQIWQ)

●   [支付宝研究员王益老师：“学好语文，才能写好代码”（很多观点对写论文同样适用）](https://zhuanlan.zhihu.com/p/157243326)

●   [哈尔滨工业大学刘一佳博士的NLPCC-2018报告：论文写作的易读性原则](http://yjliu.net/cv/res/2018-08-19-nlpcc-sws.compressed.pdf)

●   [上海交通大学张倬胜博士整理的写作建议](https://github.com/cooelf/PaperWritingTips)

●   [TTIC石昊悦博士：如何优雅地（用TeX）写AI论文](https://zhuanlan.zhihu.com/p/103519006)

●   [夕小瑶的卖萌屋：11 个好用的科研工具推荐！工作效率提升 max！](https://mp.weixin.qq.com/s/YaPYZvd12Xxgz1Y1L9Rzuw)

●   [夕小瑶的卖萌屋：吐血整理：论文写作中注意这些细节，能显著提升成稿质量](https://mp.weixin.qq.com/s/1ykqoLWjy3WhczAvb_eOoQ)

●   [Deepmind Chris Dyer 等老师：关于NLP论文中公式的建议](http://karlstratos.com/teaching/cs445fall20/short-guide-typesetting.pdf)

●   [Google Brain的Bo Chang老师的LaTeX Tips](https://bochang.me/blog/posts/latex/)

●   [如何让摘要吸引人？Nature论文摘要模板值得收藏](https://zhuanlan.zhihu.com/p/158574876)

●   [一个Notation的重要参考](https://www.deeplearningbook.org/contents/notation.html)

●   [synercys/annotated_latex_equations：Examples of how to create colorful, annotated equations in Latex using Tikz.](https://github.com/synercys/annotated_latex_equations)

●   [acmi-lab/cmu-10717-the-art-of-the-paper: Official repository for CMU Machine Learning Department&#39;s 10717: &#34;The Art of the Paper&#34;. (github.com)](https://github.com/acmi-lab/cmu-10717-the-art-of-the-paper)

●   [acl-org/aclpubcheck: Tools for checking ACL paper submissions](https://github.com/acl-org/aclpubcheck)

●   [dspinellis/latex-advice: Advice for writing LaTeX documents](https://github.com/dspinellis/latex-advice)

●   [Graham Neubig：How to Read/Write an International Conference Paper](http://www.phontron.com/slides/neubig15paperwriting.pdf)

●   [Karl Whelan：Writing Tips for PhD Theses](https://www.karlwhelan.com/Teaching/PhD/phd-writing-talk.pdf)

●   [Karl Whelan：Tips for Preparing and Publishing Research Papers](https://www.karlwhelan.com/Teaching/isne_talk_sep07.pdf)

## <img src="./pics/icon/organizer.png" width="25" />组织者列表

感谢以下同学对本项目进行组织与指导

<a href="https://github.com/Erutan-pku"> <img src="pics/profile/Erutan-pku.png"  width="80" >  </a> 
<a href="https://github.com/cooelf">  <img src="pics/profile/Zhousheng Zhang.png"  width="80" ></a> 
<a href="https://github.com/SivilTaram">  <img src="pics/profile/Qian.png"  width="80" ></a> 
<a href="https://github.com/liucongg">  <img src="pics/profile/logCong.png"  width="80" > </a> 
<a href="https://github.com/yhshu">  <img src="pics/profile/yiheng.png"  width="80" >  </a> 
<a href="https://github.com/LooperXX">  <img src="pics/profile/Xiao Xu.png"  width="80" >  </a> 
<a href="https://github.com/kokolerk">  <img src="pics/profile/jiaqi.png"  width="80" >  </a> 
<a href="https://github.com/yizhen20133868">  <img src="pics/profile/Libo Qin.png"  width="80" > </a> 


## <img src="./pics/icon/heart.png" width="25" />贡献者列表

感谢以下同学对本项目的支持与贡献

<a href="https://github.com/Erutan-pku">  <img src="pics/profile/Erutan-pku.png"  width="80" /></a> 
<a href="https://github.com/cooelf">  <img src="pics/profile/Zhousheng Zhang.png"  width="80" /></a> 
<a href="https://github.com/SivilTaram">  <img src="pics/profile/Qian.png"  width="80" /></a> 
<a href="https://github.com/liucongg">  <img src="pics/profile/logCong.png"  width="80" /></a> 
<a href="https://github.com/yhshu">  <img src="pics/profile/yiheng.png"  width="80" /></a> 
<a href="https://github.com/LooperXX">  <img src="pics/profile/Xiao Xu.png"  width="80" /></a>
<a href="https://github.com/kokolerk">  <img src="pics/profile/jiaqi.png"  width="80" /></a> 
<a href="https://github.com/yizhen20133868">  <img src="pics/profile/Libo Qin.png"  width="80" /></a> 
<a href="https://github.com/HMJiangGatech">  <img src="pics/profile/HaomingJiang.png"  width="80" /></a> 
<a href="https://github.com/jiaruonan">  <img src="pics/profile/JiaRuonan.png"  width="80" /></a> 
<a href="https://github.com/Yutong-Zhou-cv">  <img src="pics/profile/YutongZhou.png"  width="80" /></a> 
<a href="https://github.com/wangcongrobot">  <img src="pics/profile/CongWang.png"  width="80" /></a> 
<a href="https://github.com/bright2013">  <img src="pics/profile/bright2013.png"  width="80" /></a> 
