Download Link: https://assignmentchef.com/product/solved-math5473-homework-1-pca-and-mds
<br>



<ol>

 <li><em>PCA experiments: </em>Take any digit data ( ‘0’,…,‘9’), or all of them, from website http://www-stat.stanford.edu/~tibs/ElemStatLearn/datasets/zip.digits/ and perform PCA experiments with Matlab or other languages (e.g. ipynb) you are familiar:

  <ul>

   <li>Set up data matrix <em>X </em>= (<em>x</em><sub>1</sub><em>,…,x<sub>n</sub></em>) ∈ R<em><sup>p</sup></em><sup>×<em>n</em></sup>;</li>

   <li>Compute the sample mean ˆ<em>µ<sub>n </sub></em>and form <em>X</em><sup>˜ </sup>= <em>X </em>− <em>eµ</em>ˆ<em><sup>T</sup><sub>n</sub></em>;</li>

   <li>Compute top <em>k </em>SVD of <em>X</em><sup>˜ </sup>= <em>US<sub>k</sub>V <sup>T</sup></em>;</li>

   <li>Plot eigenvalue curve, i.e. <em>i </em> <em>λ<sub>i</sub></em>(Σ<sup>ˆ</sup><em><sub>n</sub></em>)<em>/tr</em>(Σ<sup>ˆ</sup><em><sub>n</sub></em>) (<em>i </em>= 1<em>,…,k</em>), with top-<em>k </em>eigenvalue <em>λ<sub>i </sub></em>for sample covariance matrix , which gives you explained variation of data by principal components;</li>

   <li>Use imshow to visualize the mean and top-<em>k </em>principle components as <em>left </em>singular vectors <em>U </em>= [<em>u</em><sub>1</sub><em>,…,u<sub>k</sub></em>];</li>

   <li>For <em>k </em>= 1, order the images (<em>x<sub>i</sub></em>) (<em>i </em>= 1<em>,…,n</em>) according to the top first <em>right </em>singular vector, <em>v</em><sub>1</sub>, in an ascending order of <em>v</em><sub>1</sub>(<em>i</em>);</li>

   <li>For <em>k </em>= 2, scatter plot (<em>v</em><sub>1</sub><em>,v</em><sub>2</sub>) and select a grid on such a plane to show those images on the grid (e.g. Figure 14.23 in book [ESL]: Elements of Statistical Learning).</li>

   <li>* You may try the parallel analysis with permutation test to see how many significantprinciple components you will obtain.</li>

  </ul></li>

 <li><em>MDS of cities: </em>Go to the following website <a href="http://www.geobytes.com/citydistancetool.htm">http://www.geobytes.com/citydistancetool.htm </a>Perform the following experiment.

  <ul>

   <li>Input a few cities (no less than 7) in your favorite, and collect the pairwise <em>air traveling </em>distances shown on the website in to a matrix <em>D</em>;</li>

   <li>Make your own codes of Multidimensional Scaling algorithm for <em>D</em>;</li>

   <li>Plot the normalized eigenvalues <em>λ<sub>i</sub>/</em>(<sup>P</sup><em><sub>i </sub>λ<sub>i</sub></em>) in a descending order of magnitudes, analyze your observations (did you see any negative eigenvalues? if yes, why?);</li>

  </ul></li>

</ol>

1

<em>Homework 1. PCA and MDS                                                                                                                                                       </em>2

<ul>

 <li>Make a scatter plot of those cities using top 2 or 3 eigenvectors, and analyze yourobservations.</li>

</ul>

<ol start="3">

 <li><em>Positive Semi-definiteness: </em>Recall that a <em>n</em>-by-<em>n </em>real symmetric matrix <em>K </em>is called positive semi-definite (<em>s.d. </em>or 0) iff for every <em>x </em>∈ R<em><sup>n</sup></em>, <em>x<sup>T</sup>Kx </em>≥ 0.

  <ul>

   <li>Show that 0 if and only if its eigenvalues are all nonnegative.</li>

   <li>Show that <em>d<sub>ij </sub></em>= <em>K<sub>ii</sub></em>+<em>K<sub>jj </sub></em>−2<em>K<sub>ij </sub></em>is a squared distance function, <em>e. </em>there exists vectors <em>u<sub>i</sub>,v<sub>j </sub></em><sup>∈ </sup>R<em><sup>n </sup></em>(1 ≤ <em>i,j </em>≤ <em>n</em>) such that <em>d<sub>ij </sub></em>= k<em>u<sub>i </sub></em>− <em>u<sub>j</sub></em>k<sup>2</sup>.</li>

   <li>Let <em>α </em>∈ R<em><sup>n </sup></em>be a signed measure s.t. <sup>P</sup><em><sub>i </sub>α<sub>i </sub></em>= 1 (or <em>e<sup>T</sup>α </em>= 1) and <em>H<sub>α </sub></em>= <em>I </em>− <em>eα<sup>T </sup></em>be the Householder centering matrix. Show that 0 for matrix <em>D </em>= [<em>d<sub>ij</sub></em>].</li>

   <li>If 0 and), show that 0 (elementwise sum), and 0 (Hadamard product or elementwise product).</li>

  </ul></li>

 <li><em>Distance: </em>Suppose that <em>d </em>: R<em><sup>p </sup></em>× R<em><sup>p </sup></em>→ R is a distance function.

  <ul>

   <li>Is <em>d</em><sup>2 </sup>a distance function? Prove or give a counter example.</li>

  </ul></li>

</ol>

√

<ul>

 <li>Is <em>d </em>a distance function? Prove or give a counter example.</li>

</ul>

<ol start="5">

 <li><sup>∗</sup><em>Singular Value Decomposition: </em>The goal of this exercise is to refresh your memory about the singular value decomposition and matrix norms. A good reference to the singular value decomposition is Chapter 2 in this book:</li>

</ol>

<em>Matrix Computations</em>, Golub and Van Loan, 3rd edition.

<ul>

 <li><em>Existence: </em>Prove the existence of the singular value decomposition. That is, show that if <em>A </em>is an <em>m</em>×<em>n </em>real valued matrix, then <em>A </em>= <em>U</em>Σ<em>V <sup>T</sup></em>, where <em>U </em>is <em>m</em>×<em>m </em>orthogonal matrix, <em>V </em>is <em>n</em>×<em>n </em>orthogonal matrix, and Σ = diag(<em>σ</em><sub>1</sub><em>,σ</em><sub>2</sub><em>,…,σ<sub>p</sub></em>) (where <em>p </em>= min{<em>m,n</em>}) is an <em>m</em>×<em>n </em>diagonal matrix. It is customary to order the singular values in decreasing order: <em>σ</em><sub>1 </sub>≥ <em>σ</em><sub>2 </sub>≥ <em>… </em>≥ <em>σ<sub>p </sub></em>≥ 0. Determine to what extent the SVD is unique. (See Theorem 2.5.2, page 70 in Golub and Van Loan).</li>

 <li><em>Best rank-k approximation – operator norm: </em>Prove that the “best” rank-<em>k </em>approximation of a matrix in the operator norm sense is given by its SVD. That is, if <em>A </em>= <em>U</em>Σ<em>V <sup>T </sup></em>is the SVD of <em>A</em>, then <em>A<sub>k </sub></em>= <em>U</em>Σ<em><sub>k</sub>V <sup>T </sup></em>(where Σ<em><sub>k </sub></em>= diag(<em>σ</em><sub>1</sub><em>,σ</em><sub>2</sub><em>,…,σ<sub>k</sub>,</em>0<em>,…,</em>0) is a diagonal matrix containing the largest <em>k </em>singular values) is a rank-<em>k </em>matrix that satisfies</li>

</ul>

k<em>A </em>− <em>A<sub>k</sub></em>k =         min       k<em>A </em>− <em>B</em>k<em>.</em>

rank(<em>B</em>)=<em>k</em>

(Recall that the operator norm of <em>A </em>is k<em>A</em>k = max<sub>k<em>x</em>k=1 </sub>k<em>Ax</em>k. See Theorem 2.5.3 (page 72) in Golub and Van Loan).

<ul>

 <li><em>Best rank-k approximation – Frobenius norm: </em>Show that the SVD also provides the best rank-<em>k </em>approximation for the Frobenius norm, that is, <em>A<sub>k </sub></em>= <em>U</em>Σ<em><sub>k</sub>V <sup>T </sup></em>satisfies</li>

</ul>

k<em>A </em>− <em>A<sub>k</sub></em>k<em><sub>F </sub></em>=          min        k<em>A </em>− <em>B</em>k<em><sub>F</sub>.</em>

rank(<em>B</em>)=<em>k</em>

<em>Homework 1. PCA and MDS                                                                                                                                                       </em>3

<ul>

 <li><em>Schatten p-norms: </em>A matrix norm k · k that satisfies</li>

</ul>

k<em>QAZ</em>k = k<em>A</em>k<em>,</em>

for all <em>Q </em>and <em>Z </em>orthogonal matrices is called a unitarily invariant norm. The Schatten <em>p</em>-norm of a matrix <em>A </em>is given by the <em>`<sub>p </sub></em>norm (<em>p </em>≥ 1) of its vector of singular values, namely,

<em>.</em>

Show that the Schatten <em>p</em>-norm is unitarily invariant. Note that the case <em>p </em>= 1 is sometimes called the nuclear norm of the matrix, the case <em>p </em>= 2 is the Frobenius norm, and <em>p </em>= ∞ is the operator norm.

<ul>

 <li><em>Best rank-k approximation for unitarily invariant norms: </em>Show that the SVD provides the best rank-<em>k </em>approximation for any unitarily invariant norm. See also 7.4.51 and</li>

</ul>

7.4.52 in:

<em>Matrix Analysis</em>, Horn and Johnson, Cambridge University Press, 1985.

<ul>

 <li><em>Closest rotation: </em>Given a square <em>n </em>× <em>n </em>matrix <em>A </em>whose SVD is <em>A </em>= <em>U</em>Σ<em>V <sup>T</sup></em>, show that its closest (in the Frobenius norm) orthogonal matrix <em>R </em>(satisfying <em>RR<sup>T </sup></em>= <em>R<sup>T</sup>R </em>= <em>I</em>) is given by <em>R </em>= <em>UV <sup>T</sup></em>. That is, show that</li>

</ul>

<em>,</em>

where <em>A </em>= <em>U</em>Σ<em>V <sup>T</sup></em>. In other words, <em>R </em>is obtained from the SVD of <em>A </em>by dropping the diagonal matrix Σ. Use this observation to conclude what is the optimal rotation that aligns two sets of points <em>p</em><sub>1</sub><em>,p</em><sub>2</sub><em>,…,p<sub>n </sub></em>and <em>q</em><sub>1</sub><em>,…,q<sub>n </sub></em>in R<em><sup>d</sup></em>, that is, find <em>R </em>that minimizes . See also (the papers are posted on course website):

<ul>

 <li>[Arun87] Arun, K. S., Huang, T. S., and Blostein, S. D., “Least-squares fitting of two 3-D point sets”, <em>IEEE Transactions on Pattern Analysis and Machine Intelligence, </em><strong>9 </strong>(5), pp. 698–700, 1987.</li>

 <li>[Keller75] Keller, J. B., “Closest Unitary, Orthogonal and Hermitian Operators to a Given Operator”, <em>Mathematics Magazine</em>, <strong>48 </strong>(4), pp. 192–197, 1975.</li>

 <li>[FanHoffman55] Fan, K. and Hoffman, A. J., “Some Metric Inequalities in the Space of Matrices”, <em>Proceedings of the American Mathematical Society</em>, <strong>6 </strong>(1), pp. 111–116, 1955.</li>

</ul>