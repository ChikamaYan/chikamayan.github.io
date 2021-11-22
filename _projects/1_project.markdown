---
layout: page
title: DualNeRF
description: a project with a background image
img: /assets/img/12.jpg
importance: 1
category: work
---

I worked with [Lourdes Agapito](http://www0.cs.ucl.ac.uk/staff/L.Agapito/) during 2020-2021 on DualNeRF, a novel view synthesis method that incorprates the extremely popular implicit neural representation, [NeRF](https://www.matthewtancik.com/nerf). DualNeRF is able to reconstruct 3D geometry and apperance of target object from a single RGB image, and does not require any expensive 3D annotations for supervision. A full Master thesis report can be found [here](/Assets/pdf/Walter_Master_Thesis.pdf).

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/arch_query_depth_with_global_high.png' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
    DualNeRF Network Architecture
</div>