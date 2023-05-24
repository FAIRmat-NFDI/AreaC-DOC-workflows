# Workflows in NOMAD

Workflows are an important aspect of data management as they enable a systematic organization of the _tasks_ performed during any Materials Science research project. We refer to a _workflow_ as a series of experiments or simulations composed of _inputs_, _outputs_, and _tasks_ performed either in serial or in parallel. Each _entry_ in NOMAD may have _workflow_ sections, describing how the (meta)data within the entry was generated. Additionally, an "overarching" workflow can be generated within its own _entry_, to define connections between multiple entries (and subworkflows) via _references_ to the corresponding entries and _sections_.

The general schema for a workflow in NOMAD (found under `nomad.datamodel.metainfo.workflow`) can be represented with the following graph:

<p align="center">
    <img src="assets/workflow-schema.png" alt="NOMAD workflow schema" title="NOMAD workflow schema">
</p>

The NOMAD workflow (blue section in the above image) is _section_ of an _entry_ in the NOMAD Archive. The workflow _subsection_`Task` contains information about each of the _tasks_ performed within the workflow. The workflow _subsection_ `TaskReference` allows to reference other _tasks_ or _workflows_. Finally, the workflow _subsection_ `Link` allows to link between _tasks_ and _sections_ within the NOMAD Archive.
<!--Still not happy with this paragraph, but if we want to show this diagram we have to somehow explain it. IMO (@JosePiarro3), the whole diagram is not understable for anyone outside FAIRmat (and probably also within FAIRmat people would have problems understanding this diagram...)-->



This documentation will show you:  <!--Extend this list according to development-->

- A simple tutorial to understand the managing and definition of custom workflows in NOMAD.
- ...