

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

 then `$x^2$` or `$x^2-\lambda+4$` will render as expected :-)


---
layout: default
---




<!-- Text can be **bold**, _italic_, or ~~strikethrough~~. -->

[Link to another page](another-page).

There should be whitespace between paragraphs.

There should be whitespace between paragraphs. We recommend including a README, or a file with information about your project.

# [](#header-1)Problem Formulation
Low rank phase retrieval (LRPR) problem, refers to recovering a low-rank matrix $\boldsymbol{X}$ from magnitude-only (phaseless) measurements of random linear projections of its
columns.
It means that, instead of a single vector $\boldsymbol{x}$ (like general phase retrieval problems), we consider a set of $q$ vectors,
$\boldsymbol{x}_1,\boldsymbol{x}_2, \dots, \boldsymbol{x}_q$, such that the $n \times q$ matrix,
\[
\boldsymbol{X}:=[\boldsymbol{x}_1,\boldsymbol{x}_2, \dots, \boldsymbol{x}_q],
\]
has rank $r \ll \min(n,q)$.
For each column $ \boldsymbol{x}_k $ of $ \boldsymbol{X} $, we observe a set of $m$ measurements of the form
<--! \begin{eqnarray} -->
\[ \boldsymbol{y}_{i,k}:= |\boldsymbol{a}_{i,k}{}'\boldsymbol{x}_k|^2, \ i = 1, 2, \dots m, \ k=1,2, \dots, q.
\label{exact_mod} \]
<--!\end{eqnarray}-->
The measurement vectors, $\boldsymbol{a}_{i,k}$, are mutually independent.

We develop two iterative algorithms for solving LRPR problem.
Both methods consist of a spectral initialization step followed by an iterative algorithm to maximize the observed data
likelihood. We obtain sample complexity bounds for our proposed initialization approach to provide a good approximation of the
true $\boldsymbol{X}$. When the rank is low enough, these bounds are significantly lower than what existing single vector phase retrieval
algorithms need. Via extensive experiments, we show that the same is also true for the proposed complete algorithms.
For more information you can see the <a href="LRPR_revise_tsp_2.pdf">paper
## [](#header-2)Header 2

> This is a blockquote following a header.
>
> When something is important enough, you do it even if the odds are not in your favor.

### [](#header-3)Header 3

```js
// Javascript code with syntax highlighting.
var fun = function lang(l) {
  dateformat.i18n = require('./lang/' + l)
  return true;
}
```

```ruby
# Ruby code with syntax highlighting
GitHubPages::Dependencies.gems.each do |gem, version|
  s.add_dependency(gem, "= #{version}")
end
```

#### [](#header-4)Header 4

*   This is an unordered list following a header.
*   This is an unordered list following a header.
*   This is an unordered list following a header.

##### [](#header-5)Header 5

1.  This is an ordered list following a header.
2.  This is an ordered list following a header.
3.  This is an ordered list following a header.

###### [](#header-6)Header 6

| head1        | head two          | three |
|:-------------|:------------------|:------|
| ok           | good swedish fish | nice  |
| out of stock | good and plenty   | nice  |
| ok           | good `oreos`      | hmm   |
| ok           | good `zoute` drop | yumm  |

### There's a horizontal rule below this.

* * *

### Here is an unordered list:

*   Item foo
*   Item bar
*   Item baz
*   Item zip

### And an ordered list:

1.  Item one
1.  Item two
1.  Item three
1.  Item four

### And a nested list:

- level 1 item
  - level 2 item
  - level 2 item
    - level 3 item
    - level 3 item
- level 1 item
  - level 2 item
  - level 2 item
  - level 2 item
- level 1 item
  - level 2 item
  - level 2 item
- level 1 item

### Small image

![](https://assets-cdn.github.com/images/icons/emoji/octocat.png)

### Large image

![](https://guides.github.com/activities/hello-world/branching.png)


### Definition lists can be used with HTML syntax.

<dl>
<dt>Name</dt>
<dd>Godzilla</dd>
<dt>Born</dt>
<dd>1952</dd>
<dt>Birthplace</dt>
<dd>Japan</dd>
<dt>Color</dt>
<dd>Green</dd>
</dl>

```
Long, single-line code blocks should not wrap. They should horizontally scroll if they are too long. This line should be long enough to demonstrate this.
```

```
The final element.
```
