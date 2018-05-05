Data Visualization Experiments
================
Muxuan Lyu & Shuai Shao
May 4, 2018

Introduction
============

Vision is the most important sense for human beings. Above **70%** of environmental information are accepted by our eyes [(Purves, 2011)](https://www.hse.ru/data/2011/06/22/1215686482/Neuroscience.pdf). Data visualization is a complicated process that involves multiple elements, among which the color plays an important role. Color conveys a lot of meaningful information unconsciously. Our brains are always trying to establish the relationship between the color and a specific meaning. According to [Lin et al. (2013)](http://eds.b.ebscohost.com.proxy.uchicago.edu/eds/pdfviewer/pdfviewer?vid=2&sid=6f030dac-b3d6-4b66-b6a2-2aba19836a59%40sessionmgr101), the “associations of colors and meanings” may be grounded in the physical appearance of objects, common metaphors, or other linguistic or cultural conventions. For instance, when visualizing the world map, we always use blue to represent oceans and use green to represent lands. Since it is obvious that human beings have the color bias that relates to specific colors and specific meanings, computer programmer sets a series of "default value" for data visualization. In this project, we plan to conduct a study to understand whether the color bias exists and how it affects our graphic perception. We will test four specific aspects that prevail in our daily life, the gender-color bias, the emotion-color bias, the political color bias, and the gradient bias. This study will deepen our understanding of color selection, perception, and interpretation in data visualization.

Participants
------------

Participants were recruited on [Amazon Mechanical Turk (MTurk)](https://www.mturk.com/) and they were invited to complete a questionnaire on Qualtrics. As described on the website, "the MTurk web service enables companies to programmatically access this marketplace and a diverse, on-demand workforce and developers can leverage this service to build human intelligence directly into their applications." Participants were required to agree on the consent form at the beginning, and those who completed the survey will receive $0.05 as rewards. \#\#Procedure The order of four studies was randomized among each participant to avoid the order effect. Participants were randomly assigned to one of the three following conditions: congruent condition, incongruent condition, and control condition for each question. In each study, participants were required to complete two multiple choices according to the graphic. Totally, they had to finish eight questions. Each question lasted five seconds and there was a two-second break between two questions. \#\#Materials

The questionnaire consisted of four studies.

### Study 1

In Study 1, we aimed to test the gender bias. Specifically, we aimed to test whether information-receivers had the bias that pink stood for females while blue stood for males.

In the congruent condition, the graphic displayed was congruent with our hypothetical bias that blue represented males and pink represented females. In the incongruent condition, the graphic displayed was incongruent with our hypothetical bias, and therefore in this condition, blue represented females and pink represented males. In the control condition, we used two colors (green and yellow) unrelated to our hypothetical bias to represent the males and females. The data were downloaded from The World Bank database.

### Study 2

It is widely acknowledged that color is a strong indicator of the emotion [(Kaya & Epps, 200)](http://eds.b.ebscohost.com.proxy.uchicago.edu/eds/pdfviewer/pdfviewer?vid=2&sid=6f030dac-b3d6-4b66-b6a2-2aba19836a59%40sessionmgr101). Each color may have several associations with different emotions, but we tended to prefer a specific color for a specific emotion. In this study, we will test the color-emotion association. The hypothetical associations are red-angry, dark green-disgust, dark grey-fear, orange-joy, blue-sadness, and purple-surprise [(Manav, 2007)](https://doi.org/10.1002/col.20294). In the study, we used simulated data (on a scale of 0-10) for different scores on the six categories of emotions.

### Study 3

In Study 3, we aimed to test the color bias for political parties. In the United States, according to [Smithonia Magazine](https://www.smithsonianmag.com/history/when-republicans-were-blue-and-democrats-were-red-104176297/#ixzz2BSTncTH4) and [the Verge](https://www.theverge.com/2012/11/6/3609534/republicans-red-democrats-blue-why-election), it was not until 2000 that red was denoted as the Republican and blue was denoted as the Democrats. In contrast to color bias of emotions which might due to evolutionary reasons, the political color bias is a relatively "novel bias" spread by social media. We wanted to test whether the political color had been a common bias in human cognition (especially for Americans) and how it affected data visualization. In the congruent condition, the graphic display was congruent with our hypothetical bias that blue represented the Democrat party and red represented the Republican party. In the incongruent condition, the matching was opposite, in which blue represented Democrats and pink represented Republicans. In the control condition, we used two colors (green and orange) unrelated to our hypothetical bias. \#\#\#Study 4 Gradient graphs are commonly used in geography and [astronomy](https://scitechdaily.com/new-video-maps-the-motions-of-structures-of-the-nearby-universe/). The gradient is typically applied to continuous variables and it denotes the degree or level. However, it remains unclear whether the direction of the color gradient could potentially affect our graph reading. In this study, we aimed to test whether the color gradient bias existed. We used a simulated density map to test the participants. We hypothesized that human-beings had the bias that low opacity denoted "lower", "fewer", or "thinner", and correspondingly, high opacity denoted "higher", "more", or "thicker".

Analysis
--------

In each study, first, we conducted a Chi-Square test to explore whether the accuracy was significantly different across three conditions. Second, we conducted an ANOVA to test the differences in reaction time of accurate responses.

Results
=======

### Gender

![](data_viz_exp_files/figure-markdown_github-ascii_identifiers/Study%201%20graphic-1.png)

Results in Study 1 indicated that both the accuracy (*χ*2=0.70, df=2, *p*=0.71) and the reaction time (*F*=0.31, df=2, *p*=0.90) did not differ across three conditions. We also proved that responses were significantly different from the random guessing. Therefore, we failed to detect the gender-color bias in the current study.

### Politics

![](data_viz_exp_files/figure-markdown_github-ascii_identifiers/study%202%20graphic-1.png)

Results in Study 2 indicated that both the accuracy (*χ*2=0.16, df=2, *p*=0.92) and the reaction time (*F*=0.27, df=2, *p*=0.76) did not differ across three conditions. We also proved that responses were significantly different from the random guessing. Therefore, we failed to detect the gender-color bias in the current study.

### Emotion

![](data_viz_exp_files/figure-markdown_github-ascii_identifiers/study%203%20graphic-1.png)

As the choices in study 3 were not binary and the correct answers to question 1 & 2 were different, we did the chi-square test separately. However, the chi-square test indicated that the difference in question 1 was significant (*χ*2=35.02, df=10, *p*&lt;0.001), while the difference in question 2 was not significant (*X*-Squared=7.46, df=10, *p*=0.68). We also proved that responses were significantly different from the random guessing. One-way ANOVA revealed no difference in reaction time of accurate responses across three conditions (*F*=0.10, df=2, *p*=0.91).

### Gradient

![](data_viz_exp_files/figure-markdown_github-ascii_identifiers/study%204%20graphic-1.png)

As the choices in study 4 are not binary and the correct answers to question 1 & 2 are different, we do the chi-square tests separately. However, the chi-square test indicates that the difference in question 1 is not significant (*χ*2=3.85, df=4, *p*=0.43), while the difference in question 2 is significant (X-Squared=14.75, df=4, p-value=0.05). One-way ANOVA reveals no difference in reaction time of accurate responses across three conditions (*F*=2.03, df=2, *p*=0.14). However, the goodness of fit test proves that responses are significantly different from the random guessing in question 1 but not in study 2.

Discussion
==========

Our study showed that people might show certain bias toward color, which could influence their perception of the graphs. However, our results differed from study to study. Both Study 1 (testing color bias for gender) and Study 2 (testing color bias for political parties) did not display any significant difference either for the accuracy of perception or reaction time for accurate responses. People’s choices in both studies were not due to chances. The results did not necessarily suggest that people did not have any color bias for gender or political parties. The reason for non-significant results might be explained by the design of the study. There were only two categories to differentiate, people’s wrong perception might be easily overridden by the information enclosed in the legend of the graph, and thus were less prone to make mistakes. Besides, people’s first perception of the graph might be subconscious and therefore difficult to detect using the format of a questionnaire. Also, as indicated in the introduction, the notion of red and blue for Republicans and Democrats was not widely accepted until late last century. Therefore, this is a novel category of color-meaning pairs that have not been formulated into a bias yet.

We demonstrated in the study of color bias for emotions that people showed differences in accuracy in one of our questions. Participants’ choices for both questions were significantly different from chances. Compared to Study 1 and 2, we had bars in six different colors with six emotions. Participants needed to process more information in order to make the correct choice within the time limit. This increase in the cognitive load might be one of the reasons that caused lower accuracy in both incongruent and control condition of question 1. However, the differences between two questions were hard to explain because the data used to generate the graphs were from simulations and we did not expect any differences between the two questions. One reason that might influence participants’ choice could be that it was conceptually hard to process the information that a person’s day was mainly dominated by fear and angry (shown in question 1) compared to sadness and fear (shown in question 2). Therefore, question 1, where the control and incongruent condition both had a greater false rate than congruent condition, showed less consistency in accuracy compared to question 2 across conditions. The reaction time again did not show any significance between conditions, which might also be due to the design of our study was not be able to detect this subtle difference in decision making.

In the study of color bias for the gradient, we did not show that people differed in either accuracy or reaction time in the three conditions. Although the accuracy of question 2 was significantly different for three conditions, people’s choices failed to show differences from chances. However, it was interesting that question 2 was the only one that showed choices were probably due to chances, which implied that the question was hard to pin down a right answer within the time limit. Therefore, we suspected that non-regular shape might be hard for people to process in addition to color information.

In conclusion, the perceptions of color were more prone to bias when people were cognitively loaded. In other words, when a graphic tries to convey a lot of information for readers to digest. People tended to use their bias for quicker processing to save the cognitive resources. However, our studies should be refined for future research in order to have a more precise conclusion of the perception bias towards color and how and when that bias affect our decision making.

Cooperation
===========

This project is accomplished by Muxuan Lyu and Shuai Shao collectively. Muxuan Lyu is responsible for **Study 1 (gender bias)** and **Study 2 (emotion bias)**. Shuai Shao is responsible for **Study 3 (political bias)** and **Study 4 (gradient bias)**. Both authors contribute to collecting data, analyzing data, and writing the report.
