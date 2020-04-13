# Support-vector-machine

Support Vector Machine

1.	Support Vector Machine Fundamentals
 
 video tutorial  for math bind  SVM https://www.youtube.com/watch?v=ax8LxRZCORU&list=PLLssT5z_DsK9JDLcT8T62VtzwyW9LNepV&index=68
 
Define the hyperplanes
H such that: w•xi +b ≥ +1 when yi =+1 w•xi +b ≤ -1 when yi = –1 d+ = the shortest distance to the closest positive point d- = the shortest distance to the closest negative point The margin (gutter) of a separating hyperplane is d+ + d–. H H1 and H2 are the planes: H1: w•xi +b = +1 H2: w•xi +b = –1 The points on the planes H1 and H2 are the tips of the Support Vectors The plane H0 is the median in between, where w•xi +b =0

Defining the separating Hyperplane
 • Form of equation defining the decision surface separating the classes is a hyperplane of the form: wTx + b = 0 – w is a weight vector – x is input vector – b is bias • Allows us to write wTx + b ≥ 0 for di = +1 wTx + b < 0 for di = –1
Some final definitions
 • Margin of Separation (d): the separation between the hyperplane and the closest data point for a given weight vector w and bias b. • Optimal Hyperplane (maximal margin): the particular hyperplane for which the margin of separation d is maximized.

Maximizing the margin 
d+ dWe want a classifier (linear separator) with as big a margin as possible. Recall the distance from a point(x0,y0) to a line: Ax+By+c = 0 is: |Ax0 +By0 +c|/sqrt(A2+B2), so, The distance between H0 and H1 is then: |w•x+b|/||w||=1/||w||, so The total distance between H1 and H2 is thus: 2/||w|| In order to maximize the margin, we thus need to minimize ||w||. With the condition that there are no datapoints between H1 and H2: xi •w+b ≥ +1 when yi =+1 xi •w+b ≤ –1 when yi =–1 Can be combined into: yi (xi •w) ≥ 1

