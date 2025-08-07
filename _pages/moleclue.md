---
permalink: /moleclue/
title: ""
author_profile: true
redirect_from: 
  - /moleclue.html
---

![Mole-Clue logo](/images/moleclue-logo.jpeg){: width="800px" }

Our mission is to modernize chemical analysis by combining GC-MS and LC-MS/MS with cutting-edge algorithms to extract deeper and more reliable insights from existing data, in a **fraction of the time**. 

## What’s The Problem?

In analytical chemistry, instrumentation is often seen as the most important piece of the puzzle. However, **data processing and analysis** is just as important. To put things into perspective, just a single GC-MS or LC-MS/MS run can result in **hundreds of megabytes** of raw instrumental data. In order to make sense of all this data, computational processing is essential. With respect to one sample, this process can be roughly split into three parts
1. Data smoothing and peak detection, centroiding and integration
2. Peak deconvolution
3. Mass spectrum analysis

The accuracy of **any** measurement, as well as the signal-to-noise ratio (S/N) and limit of detection (LOD), strongly depends on performance of the first part. The second part plays an even more important role, where a “smart enough” deconvolution algorithm can be the difference between a usable method and **additional time/effort** spent on method development. 

But the third part is arguably the most important of them all, especially in *untargeted analysis*, because the mass spectrum is the main source of information about what’s actually in the sample. Unfortunately, the coverage of spectral libraries, such as the NIST GC-MS library, is **highly limited**. Not only is this an issue for identifying compounds not in the library, but standard library search methods can also result in **false positive** or **missed** matches. 

To manage these problems, the analyst must spend a considerable amount of time **manually** looking at specific chromatographic peaks, individual mass peaks in a mass spectrum, and the returned library hits, to ensure validity of the analysis results. Not only does this slow **turnaround** per sample, but the possible **scope** of compounds detectable during analysis is restricted, since this painstaking process must be undertaken to validate the detection of each compound. These problems are *not* new, and have been around since the advent of GC-MS and LC-MS methods. Software from instrumentation vendors promise to help, but are often rigid, difficult to use, opaque, and rely on outdated algorithms from 30 or even 40 years ago. 

## What We Do

That’s why we take a **software-first** approach to chemical identification, improving the reliability and turn around time of GC-MS and LC-MS/MS analysis not with fancier instrumentation, but with tailored, in-house software built on **cutting-edge** algorithmic methods. 
These methods are grounded in **PhD research conducted at the University of Western Australia**, combining deep domain knowledge in analytical chemistry with advances in signal processing, machine learning, and optimisation methods.

Our approach enables:
1. **Faster turnaround times**, unlocking new commercial opportunities for high-throughput testing and broader service offerings.
2. **Higher identification confidence**, reducing liability and improving reproducibility in regulated or risk-sensitive environments.
3. **Semi-automated data analysis**, allowing your analysts to focus on interpreting results, not manually inspecting ion currents or mass peaks.

## Not Just Another "AI Startup"

Many so-called “AI/ML solutions” in chemistry today are generic wrappers around large language models, or involve the uncritical application of standard machine learning methods, which tend to be a **poor fit** for the actual scientific problems at hand. At Mole-Clue, we believe that **domain understanding** is crucial, and that trust, interpretability, and traceability matter more than hype. That’s why our platform is built from the ground up using **explainable machine learning** and **classical algorithmic techniques**, tailored to the specific challenges of GC-MS and LC-MS/MS workflows. We prioritise transparency over black-box predictions, especially for **regulated, risk-sensitive applications** like chemical testing, where auditability and expert oversight are non-negotiable.

## Why Mole-Clue?

Since the beginning of 2021, I have been researching and developing new computational methods to analyse mass spectral data, as part of my PhD project at the University of Western Australia. But to answer the question of *why* exactly I decided to do this project, we need to go back even further, to 2019. This was during the third year of my chemistry degree, and at the time, I was doing a research project. It occurred to me that a **surprisingly large part** of the chemical analysis I did was via “pen-and-paper”. With mass spectrometry for example, I was taught to memorise arbitrary “magic numbers” (e.g. “m/z 77 = phenyl ion”), rules-of-thumb (e.g. the “nitrogen rule”), and to draw detailed fragmentation mechanisms to “guess” the analyte structure. 

Having some previous exposure to programming via various hobby projects, I quickly realised that many of the things I was taught to memorise or write down could be done **programmatically** instead. I floated this idea to some colleagues, but they were uninterested, because writing code is not part of the standard workflow of a chemist. Later on, I was fortunate enough to speak to some mathematicians and computer scientists about it, but to even communicate what the *problem* is involved too much "front-loading" of chemistry knowledge.

So, this area appeared to be stuck in limbo; the programmers didn't know enough about chemistry to solve the **right problems**, and the chemists found it hard to **communicate** what the right problem is to programmers, in a way that they could understand. This problem affects both research scientists and analytical instrumentation manufacturers (who also made software for data processing), and the result is difficult to use vendor software, an excessive amount of time spent on “manual” data analysis by chemists, and an **inability for anyone to conceive of better alternatives**. Instead, most of the attention was being directed towards improved instrumentation the moment any problem emerges (after all, that’s the manufacturers’ main product), and the myriads of gaps and inefficiencies of data analysis methods left as an afterthought, with few even being aware of the problem. 

Knowing all that, I decided that I was going to do something about it. After sharpening my mathematical and programming skills for a year with a (mostly) unrelated honours project, I decided to turn my “pet idea” into a PhD project, being fortunate enough to get funding from the Forrest Research Foundation. In these four years, I have developed:
1. A simple but significantly more efficient [algorithm](/publication/2022-03-13-Paper-1) for generating possible molecular formulae from a given mass.
2. A [method](/publication/2023-11-07-Paper-2) that can complement (or act as an alternative to) isotopic distribution simulation for assessing the validity of molecular formulae derived from mass spectra.
3. A significantly faster method for “annotating” a mass spectrum with fragments of a known (or hypothesised) structure (currently unpublished).
4. A method that can generate possible molecular structures from an input mass spectrum **without** a spectral library or structural database (currently unpublished).

Now, I want to take the methods that I’ve developed further, beyond the confines of academic publications. So, I founded Mole-Clue, with the goal of creating practical and reliable software tools that make it **substantially** easier to extract chemical insights from GC-MS and LC-MS/MS data, and dispense of the need for chemists to memorise “magic numbers” and draw fragmentation mechanisms by hand **once and for all**.

