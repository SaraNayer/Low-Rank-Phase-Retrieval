

<style TYPE="text/css">
code.has-jax {font: inherit; font-size: 100%; background: inherit; border: inherit;}
</style>
<script type="text/x-mathjax-config">
MathJax.Hub.Config({
    tex2jax: {
        inlineMath: [['$','$'], ['\\(','\\)']],
        skipTags: ['script', 'noscript', 'style', 'textarea', 'pre'] // removed 'code' entry
    }
});
MathJax.Hub.Queue(function() {
    var all = MathJax.Hub.getAllJax(), i;
    for(i = 0; i < all.length; i += 1) {
        all[i].SourceElement().parentNode.className += ' has-jax';
    }
});
</script>
<script type="text/javascript" src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>



<script type="text/x-mathjax-config">
		MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
</script>
<script type="text/javascript" async
		src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS_CHTML">
</script>

 <!-- then `$x^2$` or `$x^2-\lambda+4$` will render as expected :-) -->


<!-- --- -->
<!-- layout: default -->
<!-- --- -->




<!-- Text can be **bold**, _italic_, or ~~strikethrough~~. -->

[Web-Page](http://www.ece.iastate.edu/~sarana/index.html).  <!-- ### Small image --> ![](https://assets-cdn.github.com/images/icons/emoji/octocat.png) 

<!-- ### Large image -->

<!-- There should be whitespace between paragraphs. -->

<!-- There should be whitespace between paragraphs. We recommend including a README, or a file with information about your project. -->

# [](#header-1)Problem Formulation
Low rank phase retrieval (LRPR) problem, refers to recovering a low-rank matrix $\boldsymbol{X}$ from magnitude-only (phaseless) measurements of random linear projections of its
columns.
It means that, instead of a single vector $\boldsymbol{x}$ (like general phase retrieval problems), we consider a set of $q$ vectors,
$ \boldsymbol{x}_1,\boldsymbol{x}_2, \dots, \boldsymbol{x}_q $, such that the $n \times q$ matrix,

$ \boldsymbol{X} := [ \boldsymbol{x}_1,\boldsymbol{x}_2, \dots, \boldsymbol{x}_q ] $ , 

has rank $r \ll \min(n,q)$.
For each column $ \boldsymbol{x}_k $ of $ \boldsymbol{X} $, we observe a set of $ m $ measurements of the form

$ \boldsymbol{y}_{i,k}  :=  $
<br/>$\|     \boldsymbol{a}_{i,k}{}'  \boldsymbol{x}_k $    \|^2 $,
<br/>$ i = 1, 2, \dots m , $ <br/>
$ k=1,2, \dots, q . $

The measurement vectors, $ \boldsymbol{a}_{i,k}$, are mutually independent.

<!-- We develop two iterative algorithms for solving LRPR problem. -->
Algorithm for solving LRPR consists of a spectral initialization step followed by an iterative algorithm to maximize the observed data
likelihood. We obtain sample complexity bounds for our proposed initialization approach to provide a good approximation of the
true $\boldsymbol{X}$. When the rank is low enough, these bounds are significantly lower than what existing single vector phase retrieval
algorithms need. Via extensive experiments, we show that the same is also true for the proposed complete algorithms.
For more information you can see the <a href="https://arxiv.org/pdf/1608.04141.pdf">paper

# [](#header-2)Video Results

>
<!-- > When something is important enough, you do it even if the odds are not in your favor.-->


<h2> Original Video </h2>
<p> 
<embed src="Orig.mp4" autostart="false" height="144" width="244" />
</p>
<br/>
<br/>
<p>
<h2> Recovered video of Holloway,J. et al's Algorithm for f = 0.25 and 0.5 respectively from left </h2>
<embed src="Holloway.25.mp4" autostart="false" height="144" width="244" />
<embed src="Holloway.5.mp4" autostart="false" height="144" width="244" />
<!-- <embed src="GrayVid_Mouse.mp4" autostart="false" height="144" width="244" /> -->
</p>
<br/>
<br/>
<P>
<h2> Results of LRPR with their initialization, for f = 0.25 and 0.5 respectively from left </h2>
<embed src="LRPR.25.mp4" autostart="false" height="144" width="244" />
<embed src="LRPRtych.5.mp4" autostart="false" height="144" width="244" />
<!-- <embed src="AMT_PlaneOrigR25L3.mp4" autostart="false" height="144" width="244" /> -->
<!-- <embed src="AMT_MouseOrigR25L3.mp4" autostart="false" height="144" width="244" /> -->
</p>
<br/>
<br/>

<!-- <h3>Parameters of Experiement <h3> -->

### [](#header-4)Parameters of Experiement 
* Size of Input Video :72 * 72 * 105 
* Diameter of Apetrue : 20 
* Number of Cameras : 49 
* Type of Video : real natural video, not been low-rankified 
* Assumption of Rank : 25
<!-- *   This is an unordered list following a header. -->
<!-- *   This is an unordered list following a header. -->
<!-- *   This is an unordered list following a header. -->

<!-- ##### [](#header-5)Header 5

<!-- 1.  This is an ordered list following a header. --> 
<!-- 2.  This is an ordered list following a header. -->
<!-- 3.  This is an ordered list following a header. -->

### [](#header-5)Normalized Error of Each Algorithms

|f(rate of unders sample)| Holloway,J. et al's | LRPR-ptycho |
|:-----------------------|:--------------------|:------------|
|          1             |       0.0580        |   0.0595    |
|         0.75           |       0.1377        |   0.0592    |
|         0.50           |       0.2240        |   0.0596    |
|         0.25           |       0.3500        |   0.0604    |
|         0.05           |       0.5545        |   0.0625    |

 <!-- ### There's a horizontal rule below this.-->

<!-- * * * -->

<!-- ### Here is an unordered list: -->

<!-- *   Item foo -->
<!-- *   Item bar -->
<!-- *   Item baz -->
<!-- *   Item zip -->

<!-- ### And an ordered list:

<!-- 1.  Item one -->
<!-- 1.  Item two --> 
<!-- 1.  Item three  -->
<!-- 1.  Item four -->

<!-- ### And a nested list:

<!--- level 1 item -->
 <!-- - level 2 item -->
 <!-- - level 2 item -->
 <!--   - level 3 item -->
  <!--  - level 3 item -->
<!-- - level 1 item -->
<!--   - level 2 item -->
<!--  - level 2 item -->
 <!--  - level 2 item -->
<!-- - level 1 item -->
<!--   - level 2 item -->
<!--   - level 2 item -->
<!-- - level 1 item -->


<!-- ![](https://guides.github.com/activities/hello-world/branching.png) -->


<!-- ### Definition lists can be used with HTML syntax. -->

<!-- <dl> -->
<!-- <dt>Name</dt> -->
<!-- <dd>Godzilla</dd> -->
<!-- <dt>Born</dt> -->
<!-- <dd>1952</dd> -->
<!-- <dt>Birthplace</dt> -->
<!-- <dd>Japan</dd> -->
<!-- <dt>Color</dt> -->
<!-- <dd>Green</dd> -->
<!-- </dl> -->

 <!-- ``` -->
<!-- Long, single-line code blocks should not wrap. They should horizontally scroll if they are too long. This line should be--> <!-- long enough to demonstrate this. -->
<!-- ``` -->

<!-- ``` -->
<!-- The final element. -->
<!-- ``` -->
