---
subtitle: Multiperspective Processes Randomization and Simulation for Online and Offline Settings
hide:
   - navigation
---

# PLG - Processes and Logs Generator

** Multiperspective Processes Randomization and Simulation for Online and Offline Settings **


![Untitled](https://github.com/delas/plg/assets/867237/5d5dd159-826c-4b09-9de5-0b7176a3c5a6)

## Introduction

Evaluating process mining algorithms could require the availability of a suite of real-world business processes and their execution logs, which hardly are available.

Process Log Generator is a application capable to generate random business processes, starting from some general "complexity paramenters". PLG is also able to "execute" a given process model in order to generate a process log.

This software is designed to help researchers in the construction of a large set of processes and corresponding execution logs. This software is released with a small library which could help in the programmatical creation of processes.

## Main features

* Random process generation, with different complexity parameters
* Random process evolution (to generate slight variations of existing processes)
* Configuration of time for activities duration and time between activities (via Python scripts)
* Generation of static/dynamic data objects for multi-perspective event log generation (via Python scripts)
* Import of process from
    * PLG file format
    * BPMN files (generated from SAP Signavio)
* Export of generated processes as
    * PLG file format
    * BPMN 2.0 XML file
    * BPMN as Graphviz Dot file
    * Petri net as Graphviz Dot file
    * Petri net as LoLA file
    * Petri net as PNML file
    * Petri net as TPN file
* Generation of an event log with any number of traces
* Fine-tuned configuration of noise parameters for event log generation
* Export of the generated event log as
    * XES file (both compressed as `.xes.gz` and not compressed as `.xes`)
    * MXML file (both compressed as `.mxml.gz` and not compressed as `.mxml`)
* Generation of an infinite stream of events
* Event streams generated as MQTT-XES format (cf. <https://www.beamline.cloud/mqtt-xes/>)
* Ability to dynamically switch the process generting the events (to simulate concept drift in streams)
* Generation of noise into the stream


## Screencast

<iframe width="560" height="315" src="https://www.youtube.com/embed/t-GMV4hU_vs?si=D2DmfgbGxJHDikvh" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>


## Download

You can read or download the updated Java source code on the project GitHub (<https://github.com/delas/plg>). Sources of the old releases of PLG are still available on the old GitHub project (<https://github.com/delas/plg-old>).


[Download latest version](https://github.com/delas/plg/releases/latest){ .md-button }


PLG makes use of the following libraries:

* [`libPlg`](https://github.com/delas/libPlg): library for processes and event generation
* [`libPlgStream`](https://github.com/delas/libPlgStream): library for stream generation
* [`libPlgVisualizer`](https://github.com/delas/libPlgVisualizer): library for process visualization

Older versions of PLG:

   * PLGLib-1.4beta
       * Release date: 2011-07-22
       * [Download this release](https://github.com/delas/plg-old/releases/tag/PLGLib-1.4beta) (sources and binary)
       * Release notes:
           * `PLG-1.4-beta.zip` the application with graphic interface
           * `PLG-CLI-ProcessCreator-0.1.jar` the command line version of the random process generator
           * `PLG-CLI-LogCreator-0.1.zip` the command line version of the process simulator (and log generator)
   * PLGLib-1.2
       * [Download this release](https://github.com/delas/plg-old/releases/tag/PLGLib-1.2) (sources and binary)
   * PLGLib-1.1
       * [Download this release](https://github.com/delas/plg-old/releases/tag/PLGLib-1.1) (sources and binary)
   * PLGLib-1.0
       * [Download this release](https://github.com/delas/plg-old/releases/tag/PLGLib-1.0) (sources and binary)


## Help and Contact

You can find more information on how to use the tool and how to configure it, on the [GihHub Wiki pages](https://github.com/delas/plg/wiki). You can find all the contact information at the [author's webpage](https://andrea.burattin.net/).

## Citation

Please, cite this work as:

* Andrea Burattin. "[PLG2: Multiperspective Process Randomization with Online and Offline Simulations](https://andrea.burattin.net/publications/2016-bpm-demo)". In *Online Proceedings of the BPM Demo Track* 2016; Rio de Janeiro, Brasil; September, 18 2016; CEUR-WS.org 2016.

Other relevant publications:

* Andrea Burattin. "[PLG2: Multiperspective Processes Randomization and Simulation for Online and Offline Settings](http://arxiv.org/abs/1506.08415)". In *CoRR* abs/1506.08415, Jun. 2015.
* Andrea Burattin and Alessandro Sperduti. "[PLG: a Framework for the Generation of Business Process Models and their Execution Logs](http://andrea.burattin.net/publications/2010-bpi)". In *Proceedings of the 6th International Workshop on Business Process Intelligence* (BPI 2010); Stevens Institute of Technology; Hoboken, New Jersey, USA; September 13, [2010.10.1007/978-3-642-20511-8_20](http://dx.doi.org/10.1007/978-3-642-20511-8_20).

