# Introduction
After finishing the previous document -- Numpy Tutorial, I decided to devote this to demonstrating how to read **dataframes** using [pandas](https://pandas.pydata.org/docs/reference/io.html) and complete some related matrix computation on the extracted data.

Our input is a text corpus from [zhihu.com](https://www.zhihu.com/question/21051140) about the grand layoff wave in China in the early 90s. My aunt and uncle were once factory workers before the layoffs. When I visited my hometown, I usually lodged in their home, listening to them recount their poignant stories during that era. Therefore, despite the generation gap, I was relatively familiar with the hardship that they have been through.  

(Apology for my digression)

This notebook will demonstrate playing with a file, the rows of which would stand for documents while the columns are keywords showing up in those documents. If the number in the cell is one, that word does appear in that document; zero otherwise.


Should I have time in the future, I will explore more NLP-related topics based on this document.  

**Table of Contents**:<br>
&nbsp;&nbsp;&nbsp;1. Introduction (we are here)<br>
&nbsp;&nbsp;&nbsp;2. Import packages<br>
&nbsp;&nbsp;&nbsp;3. Use pandas to read in datasets from Excel<br>
&nbsp;&nbsp;&nbsp;4. Extract Data<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1 Slicing<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.2 Convert the dataframe into a 2-D array<br>
&nbsp;&nbsp;&nbsp;5. Extract labels<br>
&nbsp;&nbsp;&nbsp;6. Matrix algebra<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;6.1 Co-word matrix<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;6.2 Documents similarity<br>
&nbsp;&nbsp;&nbsp;7. What's next?<br>