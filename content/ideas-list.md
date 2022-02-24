---
title: "Google Summer of Code Ideas List"
ShowToc: true
---

This is a sampling of the ideas available for potential GSoC 2022 contributors - feel free to propose your own! The goal is to start from a basic fact about the world, and use data analysis, infrastructure, and open source software to make that fact accessible to the public, researchers, and policymakers, to help them create systematic change and improve health through better policy and decision-making.

A sampling of our mentors' past open source work:
* Contributions to first version of TensorFlow Probability, such as a numerically stable Bernoulli log-likelihood that has been widely used (https://www.tensorflow.org/probability/; LDAP: @jaana; [3.6k stars](https://github.com/tensorflow/probability))
* Canonical open source variational autoencoder implementation ([900+ stars](https://github.com/altosaar/variational-autoencoder/))
* Open source bioinformatics and data science for public health: [first public dataset](https://github.com/onefact/assisted-living) of 44k assisted living facilities in the US - published at the peer-reviewed NeurIPS [Machine Learning for Public Health](https://sites.google.com/nyu.edu/mlph2021) conference in December 2021 and selected for oral presentation
* We worked with [The Browser](https://thebrowser.com) to build the first open source machine learning powered newsfeed framework, and published the source code on [GitHub](https://github.com/the-browser/recommending-interesting-writing) and the [whitepaper](http://ceur-ws.org/Vol-2682/short2.pdf) describing the architecture at an Association for Computing Machinery workshop on recommender systems 
* The first open source language model validated against clinician judgment: https://arxiv.org/abs/1904.05342 ([223 stars](https://github.com/kexinhuang12345/clinicalBERT))

## Software for visualization and geospatial analysis 

Last summer our intern Anton Stengel (Princeton '23) developed several open source tools for helping bioinformatics, epidemiology, and public health policy research. First, we built and open-sourced the only dataset of assisted living facilities in the United States. These group homes are where the elderly, poor, or people with disabilities or mental illness can live and receive support for food and shelter through Medicaid. We work with policymakers, professors, and their research teams to build open source software to make this data accessible to the public and for research.

The next step of this project requires extending the visualization library that Anton built (at https://github.com/onefact/assisted-living/). The deliverable is one step toward giving access to this data to the millions of Americans eligible for governmental housing support through Medicaid.

By building software to overlay various measures onto the map of assisted living facilities, such as the [area disadvantage index](https://www.neighborhoodatlas.medicine.wisc.edu/), our open source software will help people and policymakers access this data, understand patterns in it (such as which states or counties or cities have less density of group homes), and help people navigate the broken US health care system using open source technology. The open source analysis can then be readily extended by others working on this data. 

What you'll get out of it: 

* impact: your open source web development work will be the only place where millions of Americans can access the dataset of 45k group homes that we have assembled and find a place to live that the government will pay for.

* in addition to open source, you will be given co-author credit on the results that will be published at a peer-reviewed public health/machine learning/HCI conference (we have submitted peer-reviewed papers with 10 out of 10 of the past interns doing open source development)

## Open source AI for mental health 

This project consists of building an open source framework for machine learning and mental health. Specifically, we have built models that can train clinicians during and after therapy sessions using the recordings of their voice, and transcripts of therapy sessions.  Giving therapists this type of feedback helps reduce depression and improves mental health (for example, see [this recent article](https://www.technologyreview.com/2021/12/06/1041345/ai-nlp-mental-health-better-therapists-psychology-cbt/)). You will learn how to extend this state-of-the-art language model to create an open source, extensible framework for research and clinical use. We will follow the same protocol we used to build ClinicalBERT (described in https://arxiv.org/abs/1904.05342; source code: https://github.com/kexinhuang12345/clinicalBERT).

## Open source global mental health resource

Accessing information about therapy and mental health in the United States is extremely complex, and unfortunately many companies are out to make a buck.

For example, therapy offerred through institutions such as corporations can have grave consequences on, ironically, mental health. If an employee or student voices concerns about suicidal ideation, the repercussions from their institution can be swift and severe.

therapyhandbook.org is the first open-source resource for anyone around the world can make informed decisions and understand the financial motives that influence their mental health care. Anyone can submit edits for peer-review by our team of clinical psychologists and psychiatrists for accuracy and evidence-based treatment. 

A similar effort for digital mental health apps is here: onemindpsyberguide.org and the Therapy Handbook will operate as a sister website for therapeutic modalities themselves, such as cognitive behavioral therapy, acceptance and commitment therapy, or dialectical behavioral therapy. The target audience is anyone seeking mental health care, and in addition a clear description of the financial incentives underpinning people's decision-making around therapy and treatments will also help researchers and policymakers understand patterns in the industry. 

The open source work for this project is scoped: it revolves around the design and presentation of the complex incentives that underpin mental health care access and payment in the United States. The available information will be written and peer-reviewed by our team, and will consist of clinical guidelines found on uptodate.com, literature reviews, and information about licensing procedures and certifications for different types of therapies and mental health marketing efforts (such as cognitive behavioral therapy, internal family systems, transcendental meditation, etc.).

The frontend development consists of building a scalable NextJS website for mobile- and desktop-usage, that is lightweight to be usable on older Android phones prevalent through many low- and middle-income countries. You will be working can with our team of researchers, psychologists, and psychiatrists at our partner institutions. 

## Open source geospatial map and analysis of nuclear fallout sites in the US

We are modeling this open source development work after https://projects.propublica.org/toxmap/ - we are working with partner institutions that have collected data on every nuclear testing and fallout site in the United States. The nuclear testing has had severe repercussions on tens of thousands' of families, through cancers and other health conditions. Building an interactive map with open source technologies such as leaflet.js will help anyone affected connect to other surviors and understand what factors may have influenced their health. For a description of some of the political issues surrounding this, see [this article](https://harpers.org/archive/2022/01/spent-fuel-the-risky-resurgence-of-nuclear-power/).

## Open source visualization of cancer-causing chemicals in Black women's beauty products

Through a partnership, we have conducted a literature review of 150+ scientific publications. You will be responsible for communicating the essence of the literature review through online, interactive diagrams, using [MermaidJS](https://mermaid-js.github.io/mermaid-live-editor/).

For example, this diagram illustrates the potential links between a given product and adverse health consequences:

```
graph TD
    A[Talcum Powder] -->|COC: Asbestos| B(Absorption into bloodstream)
    B --> C{Health Outcomes}
    C -->|Demographic most affected: Black Women| D[Ovarian Cancer]
    C -->|Demographic most affected: White Women| E[Mesothelioma]
    C -->|Demographic: Hispanic Women| F[Cancer]
```



## Data science & machine learning - analysis of industry documents

Through a partnership, we have access to the UCSF Industry Documents library that collect large corporations' records that relate to public health. This project consists of applying the machine learning we developed for thebrowser.com - that is currently still in use to help editors select the best long-form content for their 70k+ readers - to these industry documents. The dashboard we built for thebrowser.com is available here: http://ceur-ws.org/Vol-2682/short2.pdf - and instead of longform journalism as data, you will be responsible for training the machine learning model on the industry documents and building the open source framework that forms the backbone of this project. 

## Open source clinical decision support tools

As [Dr. Atul Gawande](https://www.newyorker.com/magazine/2007/12/10/the-checklist) writes, checklists can save lives. However, it is difficult to deploy these life-saving tools for clinical use. For this project, the deliverable is the first open source clinical decision support tool for checklists of the type that Dr. Gawande has studied. We are building this in collaboration with our partner, [intelehealth.org](https://intelehealth.org), an open source nonprofit dedicated to last-mile delivery of health care to rural India. The open source framework to be built requires a working knowledge of tools like Next.JS, HTML5, and others. 

