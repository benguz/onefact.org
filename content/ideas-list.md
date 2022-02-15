---
title: "GSoC 2022 Ideas List"
ShowToc: true
---

This is a sampling of the ideas available for potential GSoC contributors - feel free to propose your own! The goal is to start from a basic fact about the world, and use data analysis, infrastructure, and open source software to make that fact accessible to the public, researchers, and policymakers, to help them create systematic change and improve health through better policy and decision-making.

## Interactive geospatial analysis and map of assisted living

Last summer I mentored Anton Stengel (Princeton '23), and he collected the only dataset of assisted living facilities or group homes in the United States. We published the work at a premier machine learning research conference workshop on public health, and made this website: https://onefact.org/assisted-living/

Group homes are where the elderly, poor, or people with disabilities or mental illness can live and receive support for food and shelter through Medicaid. However, these vulnerable populations have little resources (for example, Anton had to file of freedom of information requests just to get a list of Medicaid-eligible housing in some states). 

In this project, you will follow these steps to turn the dataset Anton built into product usable by any of the millions of Americans eligible for governmental housing support through Medicaid: https://labs.mapbox.com/education/impact-tools/finder-with-filters/ 

This will help people and policymakers access this data, understand patterns in it (such as which states or counties or cities have less density of group homes), and help people navigate the broken US health care system using open source technology. 

What you'll get out of it: 

* impact: your work will be the only place where millions of Americans can access the dataset of 45k group homes that we have assembled and find a place to live that the government will pay for.

* the results will be published at a peer-reviewed public health/machine learning/HCI conference (I have submitted peer-reviewed papers with 10 out of 10 of the past students I have mentored in AI and computer science research)

* presenting your work at conferences and in papers will help you become a better writer, and can help land a job at a company like Google or DeepMind (where I have previously worked). In turn, this leads to flexible career options in computer science and data science. For example, I worked with Anton Stengel, Princeton class of '23 last summer, and here is the work we published at an AI conference: https://onefact.org/assisted-living/


## Machine learning for mental health 


You will learn how to train state-of-the-art language models for helping therapists understand the contents of therapy sessions. Giving therapists this type of feedback helps reduce depression and improves mental health.

What you'll get out of it: 

* skills in applying the latest machine learning research: I will help you learn and follow the steps described on this webpage: https://huggingface.co/blog/how-to-train 

* impact: your work will be used by clinicians and startups to help train therapists in how better to talk to people and improve mental health (for a description of the technology, see https://www.technologyreview.com/2021/12/06/1041345/ai-nlp-mental-health-better-therapists-psychology-cbt/)

* the results will be published at a peer-reviewed machine learning conference (I have submitted peer-reviewed papers with 10 out of 10 of the past students I have mentored in AI research)

* presenting your work at conferences and in papers will help you become a better writer, and can help land a job at a company like Google or DeepMind (where I have previously worked). In turn, this leads to flexible career options in computer science and data science. For example, I worked with Anton Stengel '23 last summer, and here is the work we published at an AI conference: https://onefact.org/assisted-living/

## Therapy Handbook

Accessing information about therapy and mental health in the United States is extremely complex, and unfortunately many companies are out to make a buck.

For example, therapy offerred through institutions such as corporations can have grave consequences on, ironically, mental health. If an employee or student voices concerns about suicidal ideation, the repercussions from their institution can be swift and severe.

therapyhandbook.org will be the first open-source resource so that anyone around the world can make informed decisions and understand the financial motives that influence their mental health care. Anyone can submit edits, but they will be peer-reviewed by our team of clinical psychologists and psychiatrists for accuracy and evidence-based treatments. 

A similar effort for digital mental health apps is here: onemindpsyberguide.org and the Therapy Handbook will operate as a sister website for therapeutic modalities themselves, such as cognitive behavioral therapy, acceptance and commitment therapy, or dialectical behavioral therapy.

You will be responsible for design and presentation of the complex incentives that underpin mental health care access and payment in the United States. The available information will be written and peer-reviewed by our team, and will consist of clinical guidelines found on uptodate.com, literature reviews, and uncovering information about licensing procedures and certifications for different types of therapies and mental health marketing efforts (such as cognitive behavioral therapy, internal family systems, transcendental meditation, etc.).

The target audience is anyone seeking mental health care, and in addition a clear description of the financial incentives underpinning people's decision-making around therapy and treatments will also help researchers and policymakers understand patterns in the industry. 

What you'll get out of it: 

* Experience developing a scalable NextJS website for mobile- and desktop-usage, that is lightweight to be usable on older Android phones prevalent through many low- and middle-income countries.
* Experience in health care, mental health, economics, and policy. If you are in New York, you can work from the hospital our team of researchers, psychologists, and psychiatrists operate out of.
* Impact: your work will be the only place where anyone in America (and the world!) can understand the true risks and benefits inherent in any decision to seek mental health care. 
* In addition to writing articles on therapyhandbook.org, a whitepaper will be published at a peer-reviewed mental health policy conference (we have submitted peer-reviewed papers with 10 out of 10 of the past students we have mentored)
* Presenting your work at conferences and in papers will help you become a better writer, and can help land a job at in the health technology industry. For example, our intern last year published at a machine learning for public health conference: https://onefact.org/assisted-living/ based on his work in open source development: https://github.com/onefact/assisted-living/

## Interactive map of nuclear fallout sites in the US

Modeled after https://projects.propublica.org/toxmap/ - we have collected data with partners on every nuclear testing and fallout site in the United States. The nuclear testing has had severe repercussions on tens of thousands' of families, through cancers and other health conditions. Building an interactive map will help anyone affected connect to other surviors. For a description of some of the political issues surrounding this, see: https://harpers.org/archive/2022/01/spent-fuel-the-risky-resurgence-of-nuclear-power/ 

## Visualizing literature reviews of cancer-causing chemicals in Black women's beauty products

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

Through a partnership, we have access to the UCSF Industry Documents library that collect large corporations' records that relate to public health. This project consists of applying the machine learning we developed for thebrowser.com - that is currently still in use to help editors select the best long-form content for their 70k+ readers - to these industry documents. The dashboard we built for thebrowser.com is available here: http://ceur-ws.org/Vol-2682/short2.pdf - and instead of longform journalism as data, you will be responsible for training the machine learning model on the industry documents.

