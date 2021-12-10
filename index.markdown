---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: page
header_img : /assets/header.jpg
---


![]({{page.header_img | relative_url}})

<br/>

[Laurent Caraffa](https://www.umr-lastig.fr/laurent-caraffa/),
[Yanis Marchand](https://www.umr-lastig.fr/yanis-marchand/),
[Mathieu Brédif](https://www.umr-lastig.fr/mathieu-bredif/),
[Bruno Vallet](https://www.umr-lastig.fr/bruno-vallet/), 
{: style="color:gray; font-size: 120%; text-align: center;"}
# Pdf
  [https://hal.archives-ouvertes.fr/hal-03380593/file/2021216131.pdf](https://hal.archives-ouvertes.fr/hal-03380593/file/2021216131.pdf)

# Abstract
 We present an out-of-core and distributed surface reconstruction algorithm which scales efficiently on arbitrarily large point clouds (with optical centres) and produces a 3D watertight triangle mesh representing the surface of the underlying scene. Surface reconstruction from a point cloud is a difficult problem and existing state of the art approaches are usually based on complex pipelines making use of global algorithms (i.e. Delaunay triangulation, graph-cut optimisation). For one of these approaches, we investigate the distribution of all the steps (in particular Delaunay triangulation and graph-cut optimisation) in order to propose a fully scalable method. We show that the problem can be tiled and distributed across a cloud or a cluster of PCs by paying a careful attention to the interactions between tiles and using Spark computing framework. We confirm the efficiency of this approach with an in-depth quantitative evaluation and the successful reconstruction of a surface from a very large data set which combines more than 350 million aerial and terrestrial LiDAR points.

# Code
Unfortunately the source code is not aviable yet :(
We did a proof a concept for the article but the program is actually a mix of Apache/Spark, c++ with CGAL... a big mess!
However, we are working to extract each brick of the pipeline and making it open source.
If you are interested in any aspect of the code, write us!

For further updates => [Github](https://github.com/lcaraffa), [Twitter](https://twitter.com/LCaraffa)

# News
 - 2021-12-10 : Page online

# References
{% highlight bibtex %}
@inproceedings{caraffa:hal-03380593,
  TITLE = {Efficiently Distributed Watertight Surface Reconstruction},
  AUTHOR = {CARAFFA, Laurent and Marchand, Yanis and Br{\'e}dif, Mathieu and Vallet, Bruno},
  URL = {https://hal.archives-ouvertes.fr/hal-03380593},
  BOOKTITLE = {2021 International Conference on 3D Vision (3DV)},
  ADDRESS = {London, United Kingdom},
  YEAR = {2021},
  MONTH = Dec,
  PDF = {https://hal.archives-ouvertes.fr/hal-03380593/file/2021216131.pdf},
  HAL_ID = {hal-03380593},
  HAL_VERSION = {v1},
}
{% endhighlight %}

{% highlight bibtex %}
@inproceedings{caraffa:hal-02535021,
  TITLE = {Tile \\& Merge: Distributed Delaunay Triangulations for Cloud Computing},
  AUTHOR = {CARAFFA, Laurent and Memari, Pooran and Yirci, Murat and Br{\'e}dif, Mathieu},
  URL = {https://hal.archives-ouvertes.fr/hal-02535021},
  BOOKTITLE = {IEEE Big Data 2019},
  ADDRESS = {Los Angeles, United States},
  YEAR = {2019},
  MONTH = Dec,
  DOI = {10.1109/BigData47090.2019.9006534},
  KEYWORDS = {Computational Geometry ; Delaunay ; Cloud computing ; Spark},
  PDF = {https://hal.archives-ouvertes.fr/hal-02535021/file/Out_of_Core_DT_Short_paper_Camera_Ready.pdf},
  HAL_ID = {hal-02535021},
  HAL_VERSION = {v1},
}
{% endhighlight %}
{% include text-expand.html %}