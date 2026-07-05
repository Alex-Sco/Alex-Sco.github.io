---
layout: page
title: Measuring Galactic CNO isotopic ratio gradients
description: with background image
img: assets/img/12.jpg
importance: 1
category: work
related_publications: true
---


The abundance ratio between carbon, Nitrogen and Oxygen and their isotopes provide key constraints in the evolution history and stellar models in the star formation regions. Combined with the inside-out scenario of our Milky Way, the abundance ratios of <sup>12</sup>C/<sup>13</sup>C, <sup>16</sup>O/<sup>18</sup>O/<sup>18</sup>O, and <sup>14</sup>N/<sup>15</sup>N show gradient along with the Galactic radius, constraint by many observations.


However, the observational CNO isotopic ratios are poorly constraint in the Galactic metal-poor outer disk, especially for the region with Galactocentric distances > 12 kpc. We are doing series of works to deriving new CNO isotopic ratios in this region with sub-mm observations towards Galactic molecular clouds with IRAM 30-m, NOEMA and ALMA data.

In addition, we are systematically reassessing the assumptions of all current works. We have found that the previous method to use CN isotopologues have several issues, and providing new <sup>12</sup>CN/<sup>13</sup>CN measurements with updated method [Sun et al. 2024](https://ui.adsabs.harvard.edu/abs/2024MNRAS.527.8151S/abstract).

The follow-up works on this topic includes: 


I am working on the 






<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/1.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/3.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Caption photos easily. On the left, a road goes through a tunnel. Middle, leaves artistically fall in a hipster photoshoot. Right, in another hipster photoshoot, a lumberjack grasps a handful of pine needles.
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This image can also have a caption. It's like magic.
</div>



<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    You can also have artistically styled 2/3 + 1/3 images, like these.
</div>

The code is simple.
Just wrap your images with `<div class="col-sm">` and place them inside `<div class="row">` (read more about the <a href="https://getbootstrap.com/docs/4.4/layout/grid/">Bootstrap Grid</a> system).
To make images responsive, add `img-fluid` class to each; for rounded corners and shadows use `rounded` and `z-depth-1` classes.
Here's the code for the last row of images above:

{% raw %}

```html
<div class="row justify-content-sm-center">
  <div class="col-sm-8 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm-4 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
```

{% endraw %}
