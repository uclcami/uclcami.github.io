---
title: "Allan Lab - Research"
layout: textlay
excerpt: "Allan Lab -- Research"
sitemap: false
permalink: /research/
---

# Research

Our overarching goal is to explore computational modelling of quantitative MRI and validation techniques to establish new non-invasive biomarkers for cancer.

An example is the VERDICT model, a biophysical model derived from a unique DWI acquisition protocol that aims to describe diffusion in tumours developed by Dr Eleftheria (Laura) Panagiotaki. It assumes that the diffusion contributions can be categorised into three primary components: vascular (isotropic restricted pseudo-diffusion), ex-tracellular–extravascular space (hindered diffusion) and intracellular water (restricted diffusion). 

![]({{ site.url }}{{ site.baseurl }}/images/respic/verdict-model.png){: style="width: 250px; float: left; margin: 0px  10px"} 

VERDICT-MRI has been shown to provide more microstructural feature information than images derived from similar models [29, 30]. It has been specifically designed to characterise prostate tissue and so is better suited to identify PCa, providing an accurate diagnosis from MRI and preventing unnecessary biopsies [31]. To understand the clinical relevance of VERDICT-MRI, we can consider the feature maps that can be derived. These include intracellular volume faction (fIC), vascular volume fraction (fVASC), extracellular-extravascular volume fraction (fEES) and cell radius (R). PCa severity is linked to the differentiation pattern of cells. Since cancerous regions have a higher cell density and larger glands, it follows that the progression of the disease will result in a higher cell density. The fIC and R maps can therefore be used to estimate cell density in the prostate and, consequently, detect PCa. Furthermore, although both fIC and R maps are required for a precise estimation of cell density, if we assume R to be constant the fIC map becomes an indicator of cell density.

![]({{ site.url }}{{ site.baseurl }}/images/respic/verdict-example.png){: style="width: 250px; float: left; margin: 0px  10px"} 

There are two main clinical trials that focus on validating VERDICT-MRI for PCa discrimination:
• INNOVATE [31] (April 2016 to December 2019): men suspected of having PCa were prospectively recruited from two centres and underwent VERDICT MRI and mpMRI before undergoing targeted biopsy. The ADC, fractional intracellular volume (FIC), and prostate-specific antigen (PSA) density of the biopsied lesions were compared between men with csPCa and those without csPCa to test the diagnostic performance of each metric.
• Histo-MRI [32] (October 2020 to October 2023): consists of a prospectively recruited cohort of men suspected of having PCa. Histological analysis of men undergoing biopsy or prostatectomy is used for biological validation of biomark- ers from VERDICT-MRI and Luminal Water Imaging that could help avoid unnecessary biopsies in men suspected of PCa.

This data has led to a series of studies that validate the VERDICT-MRI derived maps. An in-vivo validation of fIC, fEES and fVASC was presented in an abstract in 2017 [33]. Another abstract described the increased performance of fIC maps for discrimination between Gleason grades 3+3 and ≥ 3+4 when compared to ADC maps [34]. Johnston et al. also showed that fIC values outperformed ADC in differentiating Gleason 4 lesions from lower grade or healthy tissue [30], and they demonstrated high repeatability and image quality of the fIC maps. Chiou et al. showed the promise of using fully connected neural networks to classify VERDICT-MRI images into csPCa or non-csPCa [35]. Bailey et al. later investigated the effects of fixation on VERDICT parameters [36] using ex-vivo MRI, aligning the images through rigid registrations.

More recent papers have further demonstrated the usability of VERDICT-MRI derived maps. Singh et al. showed in 2022 that fIC maps were better suited for classification into csPCa and non-csPCa than ADC and PSA density levels [31]. In particular, it was the only one that was able to discriminate lesions that scored 3 on the Likert scale. Sen et al. then showed that model-based methods such as VERDICT-MRI produced significant differences between false positives and normal tissue [37]. The in-vivo maps were also validated by comparison to volume fractions derived from histology images [38], after visual co-registration. Finally, a new version of the VERDICT model was created [39]. The parameter maps derived from this model outperformed the standard VERDICT-MRI and the ADC maps in the task of Gleason grade discrimination (between 3+3, 3+4 and ≥ 3 + 4).

### ... and more.
