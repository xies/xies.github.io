---
layout: page
title: Cell-autonomous size homeostasis in mammals
description: How are cell growth and cell cycle progression coupled?
img: assets/img/publication_preview/cell_autonomous.png
importance: 1
category: science
related_publications: true
toc:
  sidebar: top
---


## Why study cell size?

Size is one of the most fundamental parameters of a cell. Yet, we do not
understand what sets a cell's size or how they maintain that size over time.

This mechanism is especially important in cell types in our bodies that are
constantly proliferating -- that is, our stem cells. Both growth and division can
change cell size, and must be coordinated to keep cell size stable.

And why does cell size stability matter? For a single cell, its size
determines the concentration of its genome, which limits how much machinery
cells can use to grow and perform their functions. In multicellular tissues, cell size
dictates how tissues are organized, how cells move, how cells touch each other,
and other physical forces driving cell behaviors.

Despite this, cell size has not yet been systematically studied in multicellular tissues.

<br>
<br>
<br>

## What we knew (about yeast) and didn't know (about mammals)

Budding yeast cells coordinate their G1-to-S cell cycle transition to cell size.
This way, two cells that were born at different sizes end up more similar in size as they
enter S phase.

However, despite more than a decade of research in cell culture models, it was
unclear whether mammalian cells coupled their cell cycle progression to their
cell growth in quite the same way. Different cell lines seemed to have different
cell size behaviors, and it was argued that for metazoan cells, the coordination
between cell growth and cell cycle mainly occurred at the _signaling_ level, and was
not autonomous to the cell.

<u>We knew next to nothing about cells <i>in vivo</i>, however</u>.
Therefore, I developed an experimental system in which I can
study cell size homeostasis in an _in vivo_ animal,
using [intravital imaging](https://xies.github.io/projects/4d_single_cell_in_vivo_imaging/) to directly observe how single cells grow and divide in the living mouse skin, in 4D.

<div class="container">
  <div class="row justify-content-md-center">
    <div class="col-lg-4">
      {% include figure.liquid loading="eager" path="assets/img/skin/dense_cyto_t0_to_basal_tracks.gif" title="imaging a mouse's skin" class="img-fluid rounded z-depth-5" %}
    </div>
  </div>
</div>

<br>
<br>
<br>

## The G1/S transition _in vivo_ is sensitive to cell size
<div class="row">
  <div class="col-4">
      {% include figure.liquid loading="eager" path="assets/img/skin/size_control_g1_length.png" title="growth curves" class="img-fluid rounded z-depth-5" %}
      {% include figure.liquid loading="eager" path="assets/img/skin/size_control_g1.png" title="growth curves" class="img-fluid rounded z-depth-5" %}
  </div>
  <div class="col-8">
    By analyzing how single cells grow <i>in vivo</i>, I found that cells that are born
    smaller spend longer in G1 phase compared to larger born cells. This longer G1
    time means they are allowed to grow more compared to their larger-born cousins. In
    comparison, the rest of the cell cycle combined (S, G2, and M phases), was
    insensitive to cell size. {% cite xie_g1_2020 %}
    <br>
    <br>
    This coordination between cell growth and the G1/S progression is very similar
    to what was observed in budding yeast, and contrary to the majority of cell culture
    models.
  </div>
</div>

<br>
<br>
<br>

## The G1/S transition happens at an autonomously-encoded cell size threshold

Clearly, cell size is influencing whether skin stem cells _in vivo_ enter S phase or not
at any given time. However, it was unclear how much influence cell size has on this
key decision, compared to the slew of other environmental signals and changes these stem cells experience every day.

 Using quantitative image analysis, I analyzed how the dividing cell's morphology
 as well as the tissue microenvironment surrounding it changed over time. Then,
 using this rich set of information of <u>cell and microenvironment morphometrics</u>, I
 built statistical models to isolate which feature can predict whether cells will enter
 the G1/S transition. {% cite xie_g1s_2024 %}

<div class="row">
  <div class="col">
      {% include figure.liquid loading="eager" path="assets/img/skin/cell_intrinsic.png" title="cell morphology" class="img-fluid rounded" %}
  </div>
  <div class="col">
      {% include figure.liquid loading="eager" path="assets/img/skin/microenvironment.png" title="tissue microenvironment dynamics" class="img-fluid rounded" %}
  </div>
</div>
<div class="row justify-content-md-center">
  <div class='col-md-6'>
      {% include figure.liquid loading="eager" path="assets/img/skin/model_schematic.png" title="modeling G1/S transition" class="img-fluid rounded" %}
  </div>
</div>
<br>
<br>
<br>


<div class="row">
  <div class="col-6">
      {% include figure.liquid loading='eager' path='/assets/img/skin/single_model.png' title='Single cell size threshold predicts G1/S' class='img-fluid rounded z-depth-5' zoomable=true %}
  </div>
  <div class="col-5">
    My models predict G1/S transition with ~90% accuracy. Surprisingly, these models
    reveal that <i>only</i> cell volume has any significant predictive power. In fact, a
    simplified model using cell volume alone performed nearly
    as well as the full model, meaning that G1 and post-G1-phases are separable by a single
    number: <b>a cell size threshold</b>.
    <br>
    <br>
    Perturbing the microenvironment using laser cell ablations did not change this cell size threshold
    in neighboring cells, despite driving faster growth rates in those neighbors.
    Therefore, this threshold is autonomous to the dividing cell.
    <br>
    <br>

  </div>
</div>

<br>
<br>
<br>

## G1/S cell size threshold accounts for ~65% of stem cell cycle heterogeneity

The _in vivo_ skin stem cell cycle is highly heterogeneous. For the mouse hindpaw, it
could be as short as 1 day or longer than 1 week. G1 phase is by far the most variable cell cycle phase _in vivo_, accounting for
96% of the total variation in cell cycle. I showed that a combination of two
factors, <u>cell size at birth</u> (how close to the threshold a cell starts at) and <u>cell growth rate</u>
(how fast a cell approaches the threshold), can accurately predict the total
duration of G1.

<div class="container">
  <div class="row justify-content-md-center">
    <div class="col-md-5">
      {% include figure.liquid loading="eager" path="assets/img/skin/predict_g1.png" title="G1/S cell size threshold" class="img-fluid rounded z-depth-5" %}
    </div>
  </div>
</div>

<br>
<br>
<br>
<br>

## Conclusion
The highly heterogeneous cell cycles of adult stem cells _in vivo_ are
due mainly to cell size homeostasis mechanisms. That is to say, the cell cycle progression
_in vivo_ is stringently coupled to cell size, and variation in cell cycle length
serves to maintain uniformity in cell size. _Why_ cell size uniformity needs to be actively
maintained, however, is still a mystery.

<br>
<br>
<br>
<br>
