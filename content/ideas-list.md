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

## Software for Visualization and Geospatial Analysis 

### Detailed Description

Last summer our intern Anton Stengel (Princeton '23) developed several open source tools for helping bioinformatics, epidemiology, and public health policy research. First, we built and open-sourced the only dataset of assisted living facilities in the United States. These group homes are where the elderly, poor, or people with disabilities or mental illness can live and receive support for food and shelter through Medicaid. We work with policymakers, professors, and their research teams to build open source software to make this data accessible to the public and for research.

The next step of this project requires extending the visualization library that Anton built (at https://github.com/onefact/assisted-living/). The deliverable is one step toward giving access to this data to the millions of Americans eligible for governmental housing support through Medicaid.

By building software to overlay various measures onto the map of assisted living facilities, such as the [area disadvantage index](https://www.neighborhoodatlas.medicine.wisc.edu/), our open source software will help people and policymakers access this data, understand patterns in it (such as which states or counties or cities have less density of group homes), and help people navigate the broken US health care system using open source technology. The open source analysis can then be readily extended by others working on this data. 

### Expected Outcomes
* This open source web development work will be the only place where millions of Americans can access the dataset of 45k group homes that we have assembled and find a place to live that the government will pay for. It will lay the foundation for the public, policymakers, and machine learning researchers to build off of to better inform policy, understand health disparity, and help people navigate which housing is available for their elderly relatives, loved ones, or people in their lives with mental illness who need stable housing.

* In addition to the open source library, all contributors will be given co-author credit on the results that will be published at a peer-reviewed public health/machine learning/HCI conference (we have submitted peer-reviewed papers with 10 out of 10 of the past interns doing open source development).

### Skills Required / Preferred 

* Django
* OpenStreetMap 
* We are building off of this open source library for mapping health facilities: https://github.com/healthsites/healthsites/

### Possible Mentors

* [Dr. Jaan Altosaar](https://github.com/altosaar/)
* [Anton Stengel](https://github.com/antonstengel) (lead author on the original repo and paper)
* [Jeffrey Quinn](https://github.com/qwwqwwq) 
* [Professor Noémie Elhadad](https://github.com/noemieelhadad)

### Expected Size of Project

* 350 hours

### Difficulty Rating

* Medium (we have prototyped the initial version based on this [library](https://github.com/healthsites/healthsites/), what remains is to convert our [dataset](onefact.org/assisted-living) to interoperate with this)

## Open Source AI for Mental Health 

### Detailed Description

This project consists of building an open source framework for machine learning and mental health. Specifically, we have built models that can train clinicians during and after therapy sessions using the recordings of their voice, and transcripts of therapy sessions.  Giving therapists this type of feedback helps reduce depression and improves mental health (for example, see [this recent article](https://www.technologyreview.com/2021/12/06/1041345/ai-nlp-mental-health-better-therapists-psychology-cbt/)). You will learn how to extend this state-of-the-art language model to create an open source, extensible framework for research and clinical use. We will follow the same protocol we used to build ClinicalBERT (described in https://arxiv.org/abs/1904.05342; source code: https://github.com/kexinhuang12345/clinicalBERT).

### Expected Outcomes

We are basing this work off of [our GitHub repo](https://github.com/kexinhuang12345/clinicalBERT); the expected outcome is a GitHub repo consisting of a similar model -- instead of being trained on data generated by doctors, the model will be trained on data generated by therapists and their clients. This repo will allow any of the digital mental health [startups](https://onemindpsyberguide.org/) or [free services](https://cheeseburgertherapy.org/) to scale up their services off of a standard library that has been clinically validated with our collaborators at Weill Cornell Psychiatry and the Columbia University Irving Medical Center. 

### Skills Required / Preferred 

* Python
* Some familiarity with deep learning libraries such as [jax](https://github.com/google/jax), [PyTorch](https://github.com/pytorch/pytorch), or [TensorFlow](https://github.com/tensorflow/tensorflow)
* Interest in mental health
* Ideally some knowledge of [linear algebra](https://www.khanacademy.org/math/linear-algebra) and [statistics](https://www.khanacademy.org/math/statistics-probability), or a willingness to learn. We can help.

### Possible Mentors

* [Dr. Jaan Altosaar](https://github.com/altosaar/)
* [Professor Noémie Elhadad](https://github.com/noemieelhadad)

### Expected Size of Project

* 350 hours

### Difficulty Rating

* Hard (although we can base our work off of [this repo](https://github.com/kexinhuang12345/clinicalBERT) and [this tutorial](https://huggingface.co/blog/how-to-train), writing bugs in machine learning software engineering is easy, and even with our training and mentorship it will be difficult to avoid)


## Open Source Global Mental Health Resource

### Detailed Description

Accessing information about therapy and mental health in the United States is extremely complex, and unfortunately many companies are out to make a buck.

For example, therapy offerred through institutions such as corporations can have grave consequences on, ironically, mental health. If an employee or student voices concerns about suicidal ideation, the repercussions from their institution can be swift and severe.

therapyhandbook.org is the first open-source resource for anyone around the world can make informed decisions and understand the financial motives that influence their mental health care. Anyone can submit edits for peer-review by our team of clinical psychologists and psychiatrists for accuracy and evidence-based treatment. 

A similar effort for digital mental health apps is here: onemindpsyberguide.org and the Therapy Handbook will operate as a sister website for therapeutic modalities themselves, such as cognitive behavioral therapy, acceptance and commitment therapy, or dialectical behavioral therapy. The target audience is anyone seeking mental health care, and in addition a clear description of the financial incentives underpinning people's decision-making around therapy and treatments will also help researchers and policymakers understand patterns in the industry. 

The open source work for this project is scoped: it revolves around the design and presentation of the complex incentives that underpin mental health care access and payment in the United States. The available information will be written and peer-reviewed by our team, and will consist of clinical guidelines found on uptodate.com, literature reviews, and information about licensing procedures and certifications for different types of therapies and mental health marketing efforts (such as cognitive behavioral therapy, internal family systems, transcendental meditation, etc.).

The frontend development consists of building a scalable NextJS website for mobile- and desktop-usage, that is lightweight to be usable on older Android phones prevalent through many low- and middle-income countries. You will be working can with our team of researchers, psychologists, and psychiatrists at our partner institutions. 

### Expected Outcomes

* A frontend for therapyhandbook.org that operates as an open source GitHub Pages website that is mobile-friendly and ready.
* A key component is internationalization
* Importing the existing Markdown-format data from the mental health guides of our clinical partners at the [Child Mind Institute](https://childmind.org/guides/)

### Skills Required / Preferred 

* Frontend experience with NextJS (ideal) or Javascript
* Static, responsive web development experience
* Interest in mental health and low- and middle-income country humanitarian work

### Possible Mentors

* [Dr. Arno Klein](https://childmind.org/bio/arno-klein-phd/) ([GitHub](https://github.com/binarybottle))
* [Dr. Jaan Altosaar](https://github.com/altosaar/)

### Expected Size of Project

* 350 hours 

### Difficulty Rating

* Medium (Several NextJS templates exist for documentation websites that support localization, and we have a team ready to assist with user experience iteration of the frontend work)


## Open Source Interactive Geospatial Visualization of Nuclear Fallout Sites

### Detailed Description

We are modeling this open source development work after https://projects.propublica.org/toxmap/ - we are working with partner institutions that have collected data on every nuclear testing and fallout site in the United States. The nuclear testing has had severe repercussions on tens of thousands' of families, through cancers and other health conditions. Building an interactive map with open source technologies such as leaflet.js will help anyone affected connect to other surviors and understand what factors may have influenced their health. For a description of some of the political issues surrounding this, see [this article](https://harpers.org/archive/2022/01/spent-fuel-the-risky-resurgence-of-nuclear-power/).

### Expected Outcomes

* An interactive map such as https://projects.propublica.org/toxmap/ that is open source and navigable for the lay public, policymakers, data scientists, journalists, and other stakeholders 

### Skills Required / Preferred 

* Experience with open source map libraries such as Leaflet, OpenStreetMap
* Experience with Django

### Possible Mentors

* [Dr. Jesse Dunietz](https://github.com/duncanka)
* [Dr. Jaan Altosaar](https://github.com/altosaar/)

### Expected Size of Project

* 350 hours

### Difficulty Rating

* Medium (there are several open source libraries we have used to prototype, such as [this one](https://github.com/healthsites/healthsites/), so the tricky bits are getting the data on the nuclear testing and fallout sites in the right format to interoperate with these technologies)


## Open Source Visualization of Cancer-causing Chemicals in Black Women's Beauty Products

### Detailed Description
Through a partnership, we have conducted a literature review of 150+ scientific publications. You will be responsible for communicating the essence of the literature review through online, interactive diagrams, using [MermaidJS](https://mermaid-js.github.io/mermaid-live-editor/).

For example, this diagram (paste into https://mermaid-js.github.io/mermaid-live-editor/) illustrates the potential links between a given product and adverse health consequences:

```
graph TD
    A[Talcum Powder] -->|COC: Asbestos| B(Absorption into bloodstream)
    B --> C{Health Outcomes}
    C -->|Demographic most affected: Black Women| D[Ovarian Cancer]
    C -->|Demographic most affected: White Women| E[Mesothelioma]
    C -->|Demographic: Hispanic Women| F[Cancer]
```

### Expected Outcomes

* An frontend for an interactive set of MermaidJS diagrams that are based on our public health research; this will be distributed to the NGO we are partnered with and hosted as a static GitHub Pages website.

### Skills Required / Preferred 

* Experience with frontend JavaScript development
* Interest in public health 

### Possible Mentors

* [Jeff Quinn](https://github.com/qwwqwwq)
* [Dr. Jaan Altosaar](https://github.com/altosaar/)
* [Janet Nudelman, BCPP.org](https://www.linkedin.com/in/janet-nudelman-0782a72/)

### Expected Size of Project

* 150 hours

### Difficulty Rating

* Medium (there are several open source libraries we have used to prototype, such as [this one](https://github.com/healthsites/healthsites/), so the tricky bits are getting the data on the nuclear testing and fallout sites in the right format to interoperate with these technologies)


## Natural Language Processing Analysis and Dashboard for Public Health-related Industry Documents

### Detailed Description

Through a partnership, we have access to the UCSF Industry Documents library that collect large corporations' records that relate to public health. This project consists of applying the machine learning we developed for thebrowser.com - that is currently still in use to help editors select the best long-form content for their 70k+ readers - to these industry documents. The dashboard we built for thebrowser.com is available here: http://ceur-ws.org/Vol-2682/short2.pdf - and instead of longform journalism as data, you will be responsible for training the machine learning model on the industry documents and building the open source framework that forms the backbone of this project. 

### Expected Outcomes

* An interactive browser to help journalists and policymakers navigate the UCSF Industry Documents Library, based off of our prior work: https://the-browser.github.io/recommending-interesting-writing/ ([GitHub repo](https://github.com/the-browser/recommending-interesting-writing)) for the lay public, policymakers, data scientists, journalists, and other stakeholders 

### Skills Required / Preferred 

* Experience with python
* Some familiarity with machine learning libraries such as [jax](https://github.com/google/jax), [PyTorch](https://github.com/pytorch/pytorch), or [TensorFlow](https://github.com/tensorflow/tensorflow)
* Some familiarity with JavaScript and frontend development
* Interest in natural language processing tools such as as [spaCy](https://spacy.io/)

### Possible Mentors

* [Dr. Gary Ruskin](https://usrtk.org/about/gary-ruskin/)
* [Dr. Jaan Altosaar](https://github.com/altosaar/)
* [Rohan Bansal](https://rohan.page/) ([GitHub](https://github.com/rohanbansal12), lead author of the original open source library we created)

### Expected Size of Project

* 350 hours

### Difficulty Rating

* Hard (the [prototype](https://github.com/the-browser/recommending-interesting-writing) has been built, so we can base our work off of our existing work, but cleaning )

## Open Source 911 Operator Support Tools

### Detailed Description 

The [Reimagine911](https://reimaginecrisis.org/) volunteer National Action Team at [Code for America](https://codeforamerica.org/) is slated to create prototypes this summer to provide proof points of recommendations to help transform 911 systems from a tech perspective. A precursor to this work is gathering, categorizing, sorting open data sets and evaluating simple machine learning models that can best support 911 operators. A detailed description of the Reimagine911 project is [here](https://docs.google.com/presentation/d/1wp0UE8HBGe4KfrSnubLlSXx8wlBMyPlOp2DddxRpc6I/edit), and this part of the project focuses on the data science and machine learning needed to create prototypes. 

### Expected Outcomes

* An open source framework prototype recommendation systems to help 911 operators triage emergency response coordination efforts 
* The framework should support the ability to ingest, clean, and visualize the call records from the 13 cities and estimated 45 public safety answering points from around the United States
* Public dashboards using Apache Superset to increase transparency around economically-disadvantaged areas' 911 call records 

### Skills Required / Preferred 

* Experience with python
* Interest in learning business intelligence dashboard tools such as [Apache Superset](https://superset.apache.org/) that we will base our work off of 
* Interest in natural language processing tools such as as [spaCy](https://spacy.io/)

### Possible Mentors

* [Dr. Jaan Altosaar](https://github.com/altosaar/)
* [Billy Lim](https://codeforamerica.org/people/billy-lim/)

### Expected Size of Project

* 350 hours

### Difficulty Rating

* Hard (the call records data is in somewhat usable format but will take work to clean and visualize, before moving onto the prototype systems to support 911 operators in triage workflows to get callers to the right person to the right place at the right time.)

## Open source connector for FHIR API and OpenEHR 

### Detailed Description

OpenEHR is an open source standard for clinical data repositories worldwide; it has been deployed in several [countries](https://www.openehr.org/openehr_in_use/deployed_solutions/). However, there is no standard for visualizing data in OpenEHR, because of the lack of integration with a [FHIR](https://www.hl7.org/fhir/http.html) API. Specifically: OpenEHR uses an archetype query language (AQL; analogous to SQL for hierarchical data), and a FHIR API is needed to link AQL queries to data stored in enterprise resource planning (ERP) software, such as patient age, race, gender, ethnicity, and other demographics and billing information. This project will build a connector to Apache Superset between the FHIR API that links ERP data to OpenEHR data, and will enable building hospital-level analytics dashboards across the world for quality improvement, clinical documentation improvement, and clinical decision support.

### Expected Outcomes

* A connector for Apache Superset to interface between the FHIR API, enterprise resource planning software, and OpenEHR standards implementations such as EHRBase, Better, EtherCIS, etc. 

### Skills Required / Preferred 

* Experience with databases such as SQL and Postgres
* Experience with Java
* Willingness to learn AQL
* Willingness to learn about FHIR data standards 
* Interest in clinical data and machine learning

### Possible Mentors

* [Dr. Sidharth Ramesh](https://github.com/sidharthramesh)
* [Dr. Jaan Altosaar](https://github.com/altosaar/)

### Expected Size of Project

* 350 hours

### Difficulty Rating

* Hard (FHIR and OpenEHR standards are difficult to understand; however Drs. Ramesh and Altosaar have both worked extensively with Apache Superset in clinical settings)

## Open Source Clinical Decision Support

As [Dr. Atul Gawande](https://www.newyorker.com/magazine/2007/12/10/the-checklist) writes, checklists can save lives. However, it is difficult to deploy these life-saving tools for clinical use. For this project, the deliverable is the first open source clinical decision support tool for checklists of the type that Dr. Gawande has studied. We are building this in collaboration with our clinical partner, [intelehealth.org](https://intelehealth.org), an open source nonprofit dedicated to last-mile delivery of health care to rural India. The open source framework to be built requires a working knowledge of tools like Next.JS, HTML5, and others. 

### Expected Outcomes

* An open source framework for HTML5-based simple clinical decision support tools for community health workers in low- and middle-income countries
* Integration with open source clinical guideline language frameworks for interoperability, such as [GDL](https://github.com/openEHR/gdl-guideline-models#readme) and [openEHR](https://github.com/openEHR/)

### Skills Required / Preferred 

* Experience with JavaScript and HTML
* Interest in natural language processing tools such as as [spaCy](https://spacy.io/)

### Possible Mentors

* [Dr. Jaan Altosaar](https://github.com/altosaar/)
* [Lawder Paul](https://lawder.me/)
* [Priya Joshi](https://www.linkedin.com/in/priya-joshi-910b2b27/)

### Expected Size of Project

* 350 hours

### Difficulty Rating

* Hard (the [prototype](https://codepen.io/altosaar/pen/yLPjYQz) has been built based off of existing [clinical guidelines](https://www.uptodate.com/contents/covid-19-management-in-hospitalized-adults), but it will take a lot of work to support localization to Dravidian and Indo-Aryan languages like Hindi, Telugu, and Kannada.)

## Open source biofeedback for vocal physiology

### Detailed Description

Metrics from computer vision are now commodity, such as facial action unit estimation from video, or remote pulse oximetry, through to mandibular aperture. 

From such metrics, pedagogical content knowledge can be derived. For example, a simple Fourier transform can be used to inform someone with vocal pathophysiology about the strain in their vocal folds, or used to inform a singer of the rate or extent of their vibrato to help monitor their vocal health or improve their technique. 

### Expected Outcomes

* An open source, web-based, WebGL-accelerated version of Praat (https://www.fon.hum.uva.nl/praat/), that monitors pitch, analyzes rate and extent of vibrato, measures mandibular aperture, and feeds this information back in realtime to a singer, speech pathologist, vocal coach, or other interested stakeholder. It should be as easy to use as https://elsaspeak.com/en/ or https://www.duolingo.com/.

### Skills Required / Preferred 

* Experience with WebGL-accelerated code
* Experience with Javascript
* Willingness to learn computer vision libraries such as Jax, Pytorch, or TensorFlow
* Willingness to learn about vocal technique and music concepts such as fundamental frequency
* Interest in clinical speech pathology

### Possible Mentors

* [Dr. Jaan Altosaar](https://github.com/altosaar/)
* [Richard Lissemore](http://www.richardlissemore.com/)

### Expected Size of Project

* 350 hours

### Difficulty Rating

* Hard

## Open Source Clinical Decision Support

As [Dr. Atul Gawande](https://www.newyorker.com/magazine/2007/12/10/the-checklist) writes, checklists can save lives. However, it is difficult to deploy these life-saving tools for clinical use. For this project, the deliverable is the first open source clinical decision support tool for checklists of the type that Dr. Gawande has studied. We are building this in collaboration with our clinical partner, [intelehealth.org](https://intelehealth.org), an open source nonprofit dedicated to last-mile delivery of health care to rural India. The open source framework to be built requires a working knowledge of tools like Next.JS, HTML5, and others. 

### Expected Outcomes

* An open source framework for HTML5-based simple clinical decision support tools for community health workers in low- and middle-income countries
* Integration with open source clinical guideline language frameworks for interoperability, such as [GDL](https://github.com/openEHR/gdl-guideline-models#readme) and [openEHR](https://github.com/openEHR/)

### Skills Required / Preferred 

* Experience with JavaScript and HTML
* Interest in natural language processing tools such as as [spaCy](https://spacy.io/)

### Possible Mentors

* [Dr. Jaan Altosaar](https://github.com/altosaar/)
* [Lawder Paul](https://lawder.me/)
* [Priya Joshi](https://www.linkedin.com/in/priya-joshi-910b2b27/)

### Expected Size of Project

* 350 hours

### Difficulty Rating

* Hard (the [prototype](https://codepen.io/altosaar/pen/yLPjYQz) has been built based off of existing [clinical guidelines](https://www.uptodate.com/contents/covid-19-management-in-hospitalized-adults), but it will take a lot of work to support localization to Dravidian and Indo-Aryan languages like Hindi, Telugu, and Kannada.)


