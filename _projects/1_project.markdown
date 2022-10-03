---
layout: page
title: DualNeRF
description: Generalizable single view reconstruction with NeRF
img: /assets/img/depth_query_def.png
importance: 1
category: work
---

I worked with [Lourdes Agapito](http://www0.cs.ucl.ac.uk/staff/L.Agapito/) during 2020-2021 on DualNeRF, a novel view synthesis method that incorprates the extremely popular implicit neural representation, [NeRF](https://www.matthewtancik.com/nerf). DualNeRF is able to reconstruct 3D geometry and apperance of target object from a single RGB image, and does not require any expensive 3D annotations for supervision. A full Master thesis report can be found [here](/assets/pdf/Walter_Master_Thesis.pdf).

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/arch_query_depth_with_global_high.png' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
    DualNeRF Network Architecture
</div>

DualNeRF encodes the input view into a 3D feature volume, where each 1D feature vector corresponds to a pixel in the input image. A local NeRF-like decoder conditions on the pixel feature vector that contains the query point, while a global decoder conditions on the whole feature volume to give their predictions of radiance and density respectively. In the end, two set of predictions are combined using weighted sum, where weights are their densities respectively. 

Compared to the concurrent work [pixelNeRF](https://arxiv.org/abs/2012.02190), DualNeRF uses an extra global decoder to account for global rendering factors, such as illumination brightness. We also use a simplified query input to the local decoder, where the Euclidean distance between camera and query point is supplied instead of query coordinate. This gives more interpretable information to the network and forces it to fully condition on the pixel feature supplied. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/shapenet_demo.png' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
    Qualitative Evaluation on ShapeNet Car Dataset
</div>

The figure above shows a qualitative comparison among our DualNeRF, NeRF and a modified implementation of pixelNeRF, which uses smaller network and less training data due to hardware constraints.