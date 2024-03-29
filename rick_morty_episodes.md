---
title: "Rick and Morty's IMDB Scoring"
author: "Mauro"
date: "2023-12-21"
output: 
  html_document:
    keep_md: true
editor_options: 
  chunk_output_type: console
---



# Seasons


|season | mean_imdb|   sd|
|:------|---------:|----:|
|3      |      8.82| 0.62|
|2      |      8.69| 0.58|
|1      |      8.57| 0.45|
|4      |      8.37| 0.66|
|6      |      8.16| 0.37|
|5      |      7.76| 1.19|
|7      |      7.40| 1.52|

Using the mean IMDB score of every episode we conclude that best season is #3 and the lowest ranked season is the seventh. This season is also the most "volatile", with the highest standard deviation. 

![](rick_morty_episodes_files/figure-html/season_boxplot-1.png)<!-- -->

# Episodes

## Top 10 episodes


|name                                 |season | rating|
|:------------------------------------|:------|------:|
|The Ricklantis Mixup                 |3      |    9.8|
|The Rickshank Rickdemption           |3      |    9.6|
|Total Rickall                        |2      |    9.5|
|The Vat of Acid Episode              |4      |    9.4|
|Rickmurai Jack                       |5      |    9.4|
|Fear No Mort                         |7      |    9.4|
|Close Rick-counters of the Rick Kind |1      |    9.3|
|The Ricks Must Be Crazy              |2      |    9.3|
|The Wedding Squanchers               |2      |    9.3|
|Pickle Rick                          |3      |    9.3|

## Worst 10 episodes


|name                                        |season | rating|
|:-------------------------------------------|:------|------:|
|Rise of the Numbericons: The Movie          |7      |    4.4|
|Rickdependence Spray                        |5      |    5.7|
|How Poopy Got His Poop Back                 |7      |    6.0|
|Gotron Jerrysis Rickvangelion               |5      |    6.4|
|Wet Kuat Amortican Summer                   |7      |    6.5|
|Air Force Wong                              |7      |    6.8|
|Amortycan Grickfitti                        |5      |    7.0|
|Rick & Morty's Thanksploitation Spectacular |5      |    7.1|
|Claw and Hoarder: Special Ricktim's Morty   |4      |    7.3|
|The Jerrick Trap                            |7      |    7.4|

# Best director


|directed_by         | mean_imdb| count|   sd|
|:-------------------|---------:|-----:|----:|
|Eugene Huang        |      9.40|     1|   NA|
|Dominic Polcino     |      8.90|     5| 0.67|
|Stephen Sandoval    |      8.90|     3| 0.46|
|Juan Meza-León      |      8.80|     5| 0.83|
|Wes Archer          |      8.77|     3| 0.55|
|Bryan Newton        |      8.49|     8| 0.36|
|John Rice           |      8.47|     3| 0.21|
|Anthony Chun        |      8.43|     4| 0.88|
|Fill Marc Sagadraca |      8.40|     1|   NA|
|Jacob Hair          |      8.35|    12| 0.99|
|Jeff Myers          |      8.30|     2| 0.57|
|Douglas Einar Olsen |      8.05|     2| 0.35|
|Erica Hayes         |      7.98|     5| 1.36|
|Justin Roiland      |      7.90|     1|   NA|
|Juan Meza-Léon      |      7.80|     1|   NA|
|Kyounghee Lim       |      7.67|     9| 0.59|
|Douglas Olsen       |      7.10|     1|   NA|
|Lucas Gray          |      7.08|     5| 1.82|

# Best writers


|writer                | mean_imdb| count|
|:---------------------|---------:|-----:|
|Jessica Gao           |      9.30|     1|
|Mike McMahan          |      9.03|     6|
|Dan Guterman          |      8.90|     4|
|David Phillips        |      8.80|     1|
|Matt Roller           |      8.80|     1|
|Ryan Ridley           |      8.71|    10|
|Tom Kauffman          |      8.70|     6|
|Heather Anne Campbell |      8.67|     3|
|Albro Lundy           |      8.62|     6|
|Jeff Loveness         |      8.52|     6|
|Scott Marder          |      8.50|     3|
|Justin Roiland        |      8.43|     6|
|Dan Harmon            |      8.38|     4|
|Caitie Delaney        |      8.30|     1|
|Siobhan Thompson      |      8.30|     1|
|James Siciliano       |      8.21|     7|
|Michael Waldron       |      8.20|     1|
|Eric Acosta           |      8.10|     2|
|Erica Rosbe           |      8.10|     1|
|Jane Becker           |      8.10|     1|
|Sarah Carbiener       |      8.10|     1|
|Wade Randolph         |      8.10|     2|
|Cody Ziglar           |      8.00|     1|
|Jeremy Gilfor         |      8.00|     1|
|Anne Lane             |      7.88|     4|
|Alex Rubens           |      7.78|     4|
|Rob Schrab            |      6.93|     3|
|Nick Rutherford       |      6.60|     3|
|Alex Song-Xia         |      6.50|     1|
|John Harris           |      6.40|     1|

We observe that some of the top writers did only collaborate in one episode, so we'll filter the data in order to check writers of more than two episodes.


|writer                | mean_imdb| count|
|:---------------------|---------:|-----:|
|Mike McMahan          |      9.03|     6|
|Dan Guterman          |      8.90|     4|
|Ryan Ridley           |      8.71|    10|
|Tom Kauffman          |      8.70|     6|
|Heather Anne Campbell |      8.67|     3|
|Albro Lundy           |      8.62|     6|
|Jeff Loveness         |      8.52|     6|
|Scott Marder          |      8.50|     3|
|Justin Roiland        |      8.43|     6|
|Dan Harmon            |      8.38|     4|
|James Siciliano       |      8.21|     7|
|Eric Acosta           |      8.10|     2|
|Wade Randolph         |      8.10|     2|
|Anne Lane             |      7.88|     4|
|Alex Rubens           |      7.78|     4|
|Rob Schrab            |      6.93|     3|
|Nick Rutherford       |      6.60|     3|

## Rick and Morty IMDB episode scoring over time

![](rick_morty_episodes_files/figure-html/graph_over_time-1.png)<!-- -->



