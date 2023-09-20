---
layout: page
title: Shared and Distinct Neural Signatures of Feature and Spatial Attention
description: a between-subject whole-brain machine learning approach towards the predive model of the mind
img: assets/img/projects/attsig/fig1_pipeline.png
importance: 1
category: past
---

Wojciulik & Kanwisher's research(1) suggests a common involvement of the parietal cortex in visual attention (Fig. 1). In this early research, they recorded serveral participants' fMRI data and employed a univariate analysis. In the present study, we revisited the same paradigm (Fig. 2a, b) with two advancements:

- a larger cohort of participants ($$n=235$$)
- a **between-subject** whole brain machine learning approach (Fig. 2c)

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="../assets/img/projects/attsig/fig2_old_study.png" title="1999 Neuron" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Fig. 1 Common involvement of the parietal cortex in visual attention, from Wojciulik & Kanwisher, 1999
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="../assets/img/projects/attsig/fig1_pipeline.png" title="pipeline" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Fig. 2 Experiment paradigm and data analysis pipeline
</div>

We replicated the same behavioral pattern (Fig. 3a) and trained two predictive models that can not only differentiate conditions in **intra-task** scenarios, and more interstingly, in **inter-task** scenarios (Fig. 3b). This suggests both shared and distinct components exit in the **FAS** (feature attention signature) and **SAS** (spatial attention signature). 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="../assets/img/projects/attsig/fig3_model_performance.png" title="model performance" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Fig. 3 Behavioral and model performance
</div>

Fig. 4a shows the FAS and SAS at the **whole brain level**. While univariate analysis applies a boolean map with a cut-off p-value to identify the conjunction regions as the common neural subtrate, we argue that even the same region may have different pattern under different mental processes (Fig. 4a, right). When summarized at the **network level**, different portfolios emerge (Fig. 4b, left). More interesting, when retrained the predictive model on a network basis, the most prominent regions associated with the FAS were the dorsal and ventral attention networks, whereas the SAS was predominantly distributed within the visual network (Fig. 4c). 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="../assets/img/projects/attsig/fig4_whole_brain.png" title="whole brain and network" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Fig. 4 FAS and SAS at whole brain and network scale
</div>

As we have built statistical models, we further performed the following two analyses at the **cluster level**:

- Single-cluster Analysis
  - to test the sufficiency of one cluster
- 'Virtual Lesion' Analysis
  - to test the necessity of one cluster

The single-cluster analysis and the “virtual lesion” analysis revealed both shared and distinct representation patterns in FA and SA (supporting table not shown), along with the engagement of a distributed brain network in processing both forms of attention (Fig. 5a).

The distributed nature is further confirmed at the **voxel level** (Fig.5 b).

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="../assets/img/projects/attsig/fig5_cluster.png" title="cluster and voxel" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Fig. 5 Cluster and voxel level analysis
</div>

Our study challenges traditional network-centric models of attention, emphasizing **distributed** brain functioning in attention, and provides comprehensive evidence for shared and distinct neural mechanisms underlying FA and SA.

(1) Wojciulik, E., & Kanwisher, N. (1999). The generality of parietal involvement in visual attention. Neuron, 23(4), 747-764.

**See our work** at [bioRxiv](https://www.biorxiv.org/content/10.1101/2023.08.20.554014v1.abstract)