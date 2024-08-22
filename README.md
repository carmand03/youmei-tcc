# Reshaping the Chinese Ladder of Success: Documentation on Data Processing

**Abstract.** This repository contains the data and scripts related to the paper titled "Reshaping the Chinese Ladder of Success in the Era of Globalization: Family Strategies and Social Mobility of Early American-Educated Chinese (1850-1917)," published in *Twentieth-Century China*.

# Motivation 

This document describes the methodology used for extracting and analyzing data from the *Who's Who of American returned students* [Youmei tongxue lu 遊美同學錄] published by Tsing Hua College in 1917 [@tsing_hua_college_whos_1917]. The purpose is two fold (1) conduct a prosopography of the first generations of US educated Chinese (2) use this study as a test case to design a workflow for the automated extraction and multidimensional analysis of complex historical information from similar sources.   

# Primary Source 

The *Who's Who of American returned students* contains the biographies of 401 Chinese individuals who studied in the United States between 1850 and 1917. It was compiled through the initiative of the Tsinghua College Returned Students’ Information Bureau (Liumei xuesheng tongxun chu 留美學生通訊處) established in 1915. However, it is not limited to Tsinghua students, since most of the students biographed had returned by the time Tsinghua College was established in 1909. The directory was constructed by sending questionnaires directly to the students, with the assistance of students' clubs [@wu_mi__wu_1995], 153–55). 

Although the rationale for selecting the biographies remains opaque, this book nonetheless represents the most complete information available on the first generations of Chinese students in America. Each biography provides information about the students’ social and geographical background, educational curricula, subsequent professional careers, as well as their family members and sources of funding — information which is generally omitted from most biographical sources. The biographies are presented in both Chinese and English to cater to two distinct groups of readers—Chinese and American—with a dual objective in mind: first, to provide a valuable reference work for the public seeking the services of Western-educated Chinese, and second, to foster mutual understanding among the returned students themselves.This directory represents a milestone in the history of returned students in China since it represents the first attempt to construct the American-returned students (*liumei xuesheng* 留美學生, or *liumei* 留美) as a distinct, highly self-conscious social group, united by their shared educational experience in the US. 

Several digital avatars of this directory are accessible online, including on [Wikisource](https://zh.m.wikisource.org/wiki/File:Who%27s_who_of_American_returned_students_%3D_(You_Mei_tong_xue_lu_-_min_gou_liu_nian)_(IA_whoswhoofamerica00qing).pdf) and [Internet Archive](https://archive.org/details/whoswhoofamerica00qing). This research relies on the version provided by the [Institute of Modern History (IMH)](https://mhdb.mh.sinica.edu.tw/mhpeople/bookview.php?bookno=33#b33) at the Academia Sinica in Taipei, which is available for data mining with [HistText](https://bookdown.enpchina.eu/HistText_Book/) [@blouin_histtext_2023].

# Research Purposes 

The study has 3 main directions:   

  1. Analyze the social characteristics of the population to build a collective portrait of late Qing-early Republican American returned students 
  2. Uncover hidden connections among biographies based on shared affiliations or family ties 
  3. Reconstruct career paths to examine social mobility and multigenerationnal patterns of study abroad 
  
Part of this comprehensive research is published in *Twentieth-Century China* under the title "Reshaping the Chinese Ladder of Success in the Era of Globalization: Family Strategies and Social Mobility of Early American-educated Chinese (1850-1917)" as part of the special issue titled "Rethinking the Study Abroad Movement in Modern China (1850-1950s)" [@armand_reshaping_2024]. 

# Outline 

Given the scope of this research, this documentation comprises several parts based on the type of analysis and method used: 

  1. Data extraction and curation (2 scripts, one for each language)
  2. Collective portrait using multivariate and other statistical analyses 
  3. Family ties and background using network analysis (igraph) and correspondence analysis (CA) (FactominR)
  4. Affiliation networks using formal networks analysis (igraph)
  5. Career patterns using sequence analysis (TraminR)
