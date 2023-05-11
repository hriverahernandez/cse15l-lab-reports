# Lab Report 3
## Researching Command
The command that I chose for this report is the `grep` command.  
Here is the Website that I used to explore the options of `grep`: [Link](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)  
The options for `grep` that I will use are `-c`, `-v`, `-w`, and `-i`  
The file that I will be using these `grep` commands is located in `stringsearch-data/technical/plos/journal.pbio.0020001.txt`  
- `grep -c` Example 1:
  - `grep -c hi journal.pbio.0020001.txt`
  - The output was: `37`
  - The command is checking for lines that contain "hi" and only reutrn the number of lines that contain "hi" and not printing the entire line. 
This is useful as the entire line can be unnecessary information and just the line count is ecessarfy for the program.
  
- `grep -c` Example 2:
  - `grep -c world journal.pbio.0020001.txt`
  - The output was: `21`
  - The command checked for the number of lines containing the word "world". Another use for this is to check how much capacity an array must have to fit all the information conatining the word "world"
  
- `grep -v` Example 1:
  - `grep -v result journal.pbio.0020001.txt`
  - A snippet of the output was:
```
                
            North America and Europe clearly dominate the number of scientific
            publications produced annually.


        It is rather obvious that richer countries are able to invest more resources in science
        and therefore account for the largest number of publications. It is also likely that there
        is a statistical bias on the part of the SCI as a bibliometric database, since it
        represents North American and European publications far better than those of the rest of
        the world (Gibbs 1995; May 1997; Alonso and Fernández-Juricic 2001; Vohora and Vohora
        2001). But is the disparity in scientific contributions between the developed and
        developing worlds actually remaining unchanged or even increasing, as Mr. Annan has
        implied? A closer look at the trends over the last decade reveals important advances in
        developing countries. For example, Latin America and China, although representing,
        respectively, only 1.8% and 2% of scientific publications worldwide, have increased the
        number of their publications between 1990 and 1997 by 36% and 70%, respectively, which is a
        much higher percentage than the increments reached by Europe (10%) and industrial Asia
        (26%). The percentage of global scientific publications from North America actually
        decreased by 8% over the same period (UNESCO 2001).


        Publishing Trends in the Americas
        Using the SCI databases produced by the Institute for Scientific Information (ISI), as
        well as data compiled by the Red Iberoamericana de Indicadores de Ciencia y Tecnología
        (RICYT), we examined the differences in the number and proportion of scientific
        publications between the developed world and the developing world from 1990 until 2000,
        focusing on the Americas as a case study. Not surprisingly, there was a huge disparity in
        the number of publications from 1990 until 2000, with the United States contributing the
        lion's share (84.2%), followed by Canada (10.35%). Latin America as a whole contributed
        only 5.45% to the total number of scientific publications in these ten years (RICYT
        2002).
        The total number of publications, however, is not necessarily the best measure for
        assessing scientific productivity or technical advances (May 1997). More relevant
        measurements for these factors include the proportional change in the number of
        publications and the total number of publications when corrected for investment in research
        and development (May 1997). The proportional change in the number of publications, using
        1990 as a comparison, revealed that scientific publishing in Latin America increased the
        most rapidly in the Americas, far outpacing the United States and Canada (Figure 1).
        Further analyses, correcting the number of overall publications for the amount of money
        invested in research and development for each region, also show that, in contrast to both
        Canada and United States, the trend in Latin America has been an increase in relative
        output throughout the 1990s (Figure 2). Moreover, when taking into account the amount of
        research money available to researchers, Latin America actually out-published the United
        States and Canada by the year 2000 (Figure 2). Although the cost of research is undoubtedly
        cheaper in the developing world due to relatively low researcher salaries, overhead and
        other work standards, these factors do not explain the substantial increase in the number
        of publications per amount of money allocated to research and development in Latin America,
        particularly from 1995 until 2000 (Figure 2).
        Other relative indicators of scientific productivity, such as the number of publications
        picked up by the SCI in relation to the number of scientists in a particular country, also
        demonstrate that such developing regions as Latin America are making substantial
        contributions to science, despite the fact that the average proportion of gross domestic
        product (GDP) invested in science in Latin America throughout this 10-year period was only
        21% of the amount invested in United States (RICYT 2002). Indeed, this scientific
        productivity is remarkable when we compare it with the relatively low investment in science
        itself as compared with the GDP of Latin America as a whole. In fact, Albornoz (2001)
        concluded that, as a group, Latin America could afford to invest a much higher proportion
        of its resources in scientific research and development. Latin American investment in
        research and development represented only 0.59% of the regional GDP in 1998, a very weak
        effort compared with that of the United States (2.84%) and Canada (1.5%).
        Among Latin American countries, there is a high degree of variability in publication
        rate as well as in financial investment in science and technology. Some countries have
        performed particularly well. For example, Uruguay, Chile, Panama, and Cuba averaged,
        respectively, 6.8, 5.3, 5.2, and 3.4 publications per million dollars of research and
        development investment in the 10 years studied, which is notoriously high compared with
        United States (1.5) and even Canada (3.3) (RICYT 2002). Other countries, such as Costa
        Rica, Cuba, Brazil, and Chile, have invested a much greater proportion of their GDP in
        research and development than the other countries of this region (Albornoz 2001).
```

  - The command is checking for lines that don't contain "result" and prints out all lines that meet that criteria. This is useful if there is a word that you don't want included in the final results of the program.
- `grep -v` Example 2:
  - `grep -v a journal.pbio.0020001.txt`
  - A snippet of the output was:
  - ```
        serious problems not only for the scientific community in the developing countries, but for

        2002).

        regions.
        In
        However, publishing in

        world.
        
        built.
  - The command is checking for lines that don't contain the letter "a" and prints out all lines that meet that criteria. 
A useful way to use this is to exclude certain character(s) and note the effect it has when it's missing.
  
- `grep -w` Example 1:
  - `grep -w are journal.pbio.0020001.txt`
  - The output was:
```
        It is rather obvious that richer countries are able to invest more resources in science
        demonstrate that such developing regions as Latin America are making substantial
        which are mutually exclusive. It is possible that publishing in international journals as a
        regions as Latin America are falling short of reaching the top journals. In contrast, the
        American researchers are not shying away from the two top-ranked general science journals.
        Although there are outstanding scientific researchers in the developing world who
        independently are making important contributions to the international scientific community,
        they are the exception. Why, in general, do Latin American scientists often fail to reach
        possibility is that the main research agendas between both regions are somewhat different
        and that the top journals, which are published in the developed world, respond more to the
        developed regions are listed by the SCI than similar journals from developing regions
        (Gibbs 1995). Consequently, there are more high-profile regional publication opportunities
        Annan. There are many compelling reasons for the push to increase scientific input from the
        from those developing regions that are so important for these global processes. It is also
        areas of concern that are having a proportionally greater scientific and social impact upon
        them. There are now examples in which research on priority areas for the developing nations
        examples are important not only for those regions of the developing world, but are also in
            input from those developing regions that are so important for global processes.
        community, there are also reasons to be optimistic. The relative increase in the number of
        development, demonstrates that many developing countries are heading in the right
        to travel, we feel optimistic that the bridges mentioned by Mr. Annan are slowly being
```
  - The command is checking for lines that contain the word "are" and prints out all lines that meet that criteria. 
This is useful as many small words existing in larger words, and `grep` by itself cannot distinguish between them.
- `grep -w` Example 2:
  - `grep -w right journal.pbio.0020001.txt`
  - The output was:
  - ```
        development, demonstrates that many developing countries are heading in the right
  - The command is checking for lines that contain the word "right" and prints out all lines that meet that criteria. 
A way to use this would be in a dictionary as many of the small words are in the larger words, and `-w` can help you find the exact word you need.
  
- `grep -i` Example 1:
  - `grep -i SCIENCE journal.pbio.0020001.txt`
  - The output was:
```
        the clear inequalities in science between developing and developed countries and to the
        importance of reducing the inequalities in science between developed and developing
        88% of all scientific and technical publications registered by the Science Citation Index
        It is rather obvious that richer countries are able to invest more resources in science
        contributions to science, despite the fact that the average proportion of gross domestic
        product (GDP) invested in science in Latin America throughout this 10-year period was only
        productivity is remarkable when we compare it with the relatively low investment in science
        rate as well as in financial investment in science and technology. Some countries have
        funding to the most productive scientists from the national science development programs
        and global change biology) between 1990 and 2002 in both the two top general science
        Science ; with impact factors of 27.96 and 23.33, respectively) and in
        Science and
        Science and
        American researchers are not shying away from the two top-ranked general science journals.
        Science and
        ecology and environmental sciences emphasizes the overwhelming contributions of authors
        conspiracy, but rather it implies that the perception of the most important science is
        science is most interesting to them. Another consideration is that more local journals from
        developing world (Goldemberg 1998; Annan 2003). One is that science, as a discipline, would
        Brazil (Goldemberg 1998) and biomedical sciences in Cuba (Castro Díaz-Balart 2002). These
        to the sciences will be an excellent investment by developing nations in terms of
```
  - The command is checking for lines that contain the word "SCIENCE", ignoring the case, and prints out all lines that meet that criteria. 
    This is useful because many words in the internet contain a mix of upper and lower case.
- `grep -i` Example 2:
  - `grep -i BeTwEeN journal.pbio.0020001.txt`
  - The output was:
```
        the clear inequalities in science between developing and developed countries and to the
        importance of reducing the inequalities in science between developed and developing
        output between the developing and already developed countries (Gibbs 1995; May 1997;
        2001). But is the disparity in scientific contributions between the developed and
        number of their publications between 1990 and 1997 by 36% and 70%, respectively, which is a
        publications between the developed world and the developing world from 1990 until 2000,
        and global change biology) between 1990 and 2002 in both the two top general science
        possibility is that the main research agendas between both regions are somewhat different
```
  - The command is checking for lines that contain the word "BeTwEeN", ignoring the case, and prints out all lines that meet that criteria. 
    A useful application for this would be forums where people communicate as many people use interchanging cases to change the tone of a word.
