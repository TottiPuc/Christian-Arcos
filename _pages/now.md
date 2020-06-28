---
title: "Now"
layout: splash
permalink: /now/
date: 2016-03-23T11:48:41-04:00
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /images/deep.jpg
  #actions:
   # - label: "Download"
    #  url: "https://github.com/mmistakes/minimal-mistakes/"
  caption: "Deep Learning"
excerpt: "What I'm up to? I am currently working on two major projects in the two great branches of AI, speech recognition and computer vision."
intro: 
  - excerpt: '"Nothing in life is to be feared, it is only to be understood. Now is the time to understand more, so that we may fear less."  `Marie Curie`'
feature_row2:
  - image_path: /images/citrus.jpg
    alt: "hyperspectral image"
    title: "Deep Image Fusion"
    excerpt: 'Development of an optical-computational system for the fusion of depth and hyperspectral images using deep learning techniques and their application in the classification of citrus by its level of maturity.'
    #url: "#test-link"
    #btn_label: "Read More"
    #btn_class: "btn--primary"
feature_row3:
  - image_path: /images/speech.jpg
    alt: "speech recognition"
    title: "Speech Recognition system"
    excerpt: 'Speech recognition for people with amyotrophic lateral sclerosis (ALS). Which is a long-term project that I'm not ready to share yet, but you will soon notice!'
    #url: "#test-link"
    #btn_label: "Read More"
    #btn_class: "btn--primary"
feature_row4:
  - image_path: /assets/images/unsplash-gallery-image-2-th.jpg
    alt: "placeholder image 2"
    title: "Placeholder Image Center Aligned"
    excerpt: 'This is some sample content that goes here with **Markdown** formatting. Centered with `type="center"`'
    url: "#test-link"
    btn_label: "Read More"
    btn_class: "btn--primary"
---

{% include feature_row id="intro" type="center" %}

{% include feature_row id="feature_row2" type="left" %}

{% include feature_row id="feature_row3" type="right" %}

{% include feature_row id="feature_row4" type="center" %}