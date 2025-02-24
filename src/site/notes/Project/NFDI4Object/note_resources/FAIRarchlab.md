---
{"dg-publish":true,"permalink":"/project/nfdi-4-object/note-resources/fai-rarchlab/","tags":["gardenEntry"]}
---

# FAIRarchlab

## Introduction 

**FAIRarchlab** features a vibrant suite of services and laboratory standards that enable the FAIR management of analytical data in archaeometry. Our platform is dedicated to providing a comprehensive catalogue of laboratory services, metadata description for scientific instruments, standardised documentation for sample workflows and measurement properties, digital operation of laboratory tasks, and an open-access data repository (in association with Geohist Metal). With a strong foundation in community involvement and existing standards, we are committed to establishing guidelines and best practices for laboratory analytics and experiments. Our data infrastructure, powered by open-source software and tools, integrates closely with other applications and platforms through APIs, enabling seamless data sharing and a connected research ecosystem. 

## Roadmap and Milestones

```mermaid

gantt
	todayMarker off
    dateFormat  YYYY-MM-DD
    tickInterval 3month
    title       FAIRarchlab Roadmap 2025-2027: Overall
     (`excludes` accepts specific dates in YYYY-MM-DD format, days of the week ("sunday") or "weekends", but not the word "weekdays".)


    section Discovery Service
    Catelogue of Services                :sd, 2025-01-01, 17.2w
    Developing Models              :done,  sd1, 2025-01-01, 8w
    Collecting Cases              :active,  sd2, after sd1, 9.2w
    Software/Server Evaluation               :se, 2025-01-01,12.8w
    Decision on Software Architecture                 :crit, milestone, after se, 0d
    Software Architecture               :sa, after sd2,35w
    Server and Software Setup              :active, sa1,after sd2, 12w
    Backend Development              :active,  sa2, after sa1, 23w

    section ELNs
    ELN Evaluation                   :eln1, 2025-04-01,13w
    Chemotion                     :active, eln2, 2025-04-01,4.33w
    Rspace                    :active, eln3, after eln2,4.33w
    eLabFTW                     :active, eln4, after eln3,4.33w
    Decision on ELNs                 :crit, milestone, after eln4, 0d
    ELN Implementation in the DBM                   :eln5, after eln4,26.4w
    Server and Software Setup              :active, eln5,after eln4, 9w
    Workflow setup              :active, eln6,after eln5, 17.4w

    section PIDs
    DataCite IGSN               :pid1, 2025-07-01, 4.5w
    Instrument                :pid2, after pid1, 4.5w
    Schema,Vocab               :pid3, after pid1, 4.5w
    Integration with Service Software              :pid4, after pid3, 12.5w
    PID Setup Finished                :crit, milestone, after pid4, 0d
    


    section Working Groups
    TWG Device Standard                 :TWG1, 2025-01-01, 25.8w
    Metadata Schema (JSON,CSV)      :done, TWG1-1,2025-01-01  , 10w
    Vocabulary      :active, TWG1-2, after TWG1-1, 8w
    Ontology & KG      :active, TWG1-3, after TWG1-2, 7.8w
    WG White Paper                 :crit, milestone, after TWG1-3, 0d
    Preparation for a New TWG               :TWG2, 2025-09-01, 17.4w

```

```mermaid

gantt
    dateFormat  YYYY-MM-DD
    tickInterval 1month
    title       FAIRarchlab Roadmap 2026-2027: Implementation Phase
     (`excludes` accepts specific dates in YYYY-MM-DD format, days of the week ("sunday") or "weekends", but not the word "weekdays".)


    section Interface between Services 
    Integration between Discovery Service and ELN               :in, 2027-01-01,17w
    Integration between ELN and Geohist              :in1, after in, 17.5w
    Integration between DBM Services and other Platforms              :in2, after in1, 17.5w
    Interface Completed                 :crit, milestone, after in2, 0d

    section Geohist Metal
    Constructing Database (EasyDB?)      :GM1,2027-01-01  , 12w
    Integrating with other Geohist Databases :GM2, after GM1, 14w
    Geohist Metal Repo                :crit, milestone, after GM2, 0d    

```
