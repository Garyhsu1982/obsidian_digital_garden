---
{"dg-publish":true,"permalink":"/nfdi-4-objects/3-tools-and-resources/software/","noteIcon":""}
---


## Electronic Lab Notebook
### Rspace
[Github repo](https://github.com/rspace-os/rspace-docker?tab=readme-ov-file)
## elabFTW
[installation](https://doc.elabftw.net/install.html)
### Chemotion
[installation](https://chemotion.net/docs/eln/install_configure)
[DBM instance]([https://bergbau.eln.chemotion.scc.kit.edu/](https://bergbau.eln.chemotion.scc.kit.edu/))
### LabStep


## Electronic Field Notebook
### Fieldmark
[designer](https://designer.fieldmark.app/)
[conductor](https://conductor.fieldmark.app/auth/)
[Github repo](https://github.com/FAIMS/FAIMS3)
[user guide](https://docs.google.com/document/d/1DCZzca6xOqBhst1849eE6LM0aKWaISDImcSVYMiYKyY/edit?tab=t.0)

## Vocabulary/Ontology Management Software
[Opentheso](https://github.com/miledrousset/Opentheso/tree/master?tab=readme-ov-file)
Publish your own Vocabs: [1](https://blog.skohub.io/2024-03-21-skohub-pages/) [2](https://metadaten.community/t/skohub-pages-skos-publikation-auf-die-einfache-art/257)
[Skos play](https://skos-play.sparna.fr/play/)
A free software visualises thesaurus, taxonomies or controlled vocabularies expressed in [SKOS](http://www.w3.org/TR/2009/REC-skos-reference-20090818/).
[a list of controlled vocab software](https://github.com/gbv/bartoc.org/wiki/Software-for-controlled-vocabularies)
### Protégé
ontology development
Tutorial: https://cgi.csc.liv.ac.uk/~frank/teaching/comp08/protege_tutorial.pdf
Old tutorial: https://protege.stanford.edu/conference/2006/submissions/slides/OWLTutorial_Part1.pdf
official tutorial: http://protegeproject.github.io/protege/getting-started/
tutorial: https://www.michaeldebellis.com/post/new-protege-pizza-tutorial

### OntoMe
https://ontome.net/property
### [Web-Karma](https://github.com/usc-isi-i2/Web-Karma)

### Ontop
SQL database to RDF
https://ontop-vkg.org/
## Research Data Management Software
### OpenAltas
[official website](https://openatlas.eu/)
[Github repository](https://github.com/craws/OpenAtlas/blob/main/install.md)
[my own installation guide](OpenAtlas.md)
[Redmine ticketing](https://redmine.openatlas.eu/projects)) 
### Omeka software
[Omeka S](https://omeka.org/s/docs/user-manual/install/)
[Omeka Classic](https://omeka.org/classic/docs/Installation/System_Requirements/)
### Drupal-Wisski
A  content  management framework that support the editing of ontology (CDOC-CRM). publishing, and data entry. 
It is also associated with NFDI4CULTURE. 
[installation](https://wiss-ki.eu/download_and_install)
[own installation guide](Drupal-Wisski.md)
WissKI meeting 2024 ([doc](https://docs.google.com/document/d/1SX0y778HpjV35q6UoYv5q-3tSUW6jekHOwMEfI9MEYw/edit?tab=t.0)), ([miroboard](https://miro.com/app/board/uXjVLCVQWwA=/))
### Dspace
[official website](https://dspace.org/)
[wiki guide](https://wiki.lyrasis.org/display/DSPACE/Home) 
[instances](https://dspace.org/registry/)
### EasyDB-Fylr
[Fylr documentation](https://docs.fylr.io/))
**community meeting 2025 notes**: [link](https://docs.google.com/document/d/18pVGC_bQFgcOYijjlqJqB-nZDhrjmFP7Tj7PzInXapc/edit?tab=t.0#heading=h.m8w43bakqrmb)
https://heidicon.ub.uni-heidelberg.de/search
https://github.com/ssciwr/svelte-easydb-detail-view
### Codra
Digital Object Management Software
[official website](https://www.cordra.org/cordra.html) 
### Kitodo
Software to manage a digital library 
[official website](https://www.kitodo.org/en/software/about-the-software) 

### InvenioRDM
Workshop at the University of Münster [presentation](https://pad.uni-muenster.de/p/5K3B3kUsk#/). [Official Documentation](https://inveniordm.docs.cern.ch/)

You need to install 1. Devbox and 2. Docker and Docker compose


1. Devbox installieren
```
curl -fsSL https://get.jetpack.io/devbox | bash
```

2. Devbox Repo clonen & aktivieren

```
git clone git@github.com:ulbmuenster/invenio-devbox.git
cd invenio-devbox
devbox shell
```

3. InvenioRDM installieren

```
devbox run install-empty
```

4. InvenioRDM starten

```
cd my-site
invenio-cli run
```

Then, open https://127.0.0.1:5000/ in the browser
Default account: [admin@inveniosoftware.org](mailto:admin@inveniosoftware.org) Default password: 123456 


5. Customise the submission forms (change metadata profile)

garyhsu@G05-LAP-HSU:~/invenio-devbox/my-site/app_data/vocabularies$

the default installation under invenio-devbox/.venv/var/instance/assests/js you can modify
then paste it to the same folder to my-site

If you want to change forms, you

garyhsu@G05-LAP-HSU:~/invenio-devbox$ devbox sdhell
(.venv) (devbox) garyhsu@G05-LAP-HSU:~/invenio-devbox$ cd my-site/
(.venv) (devbox) garyhsu@G05-LAP-HSU:~/invenio-devbox/my-site$ invenio-cli services stop
Stopping containers...
Stopped containers.
(.venv) (devbox) garyhsu@G05-LAP-HSU:~/invenio-devbox/my-site$ exit
exit
garyhsu@G05-LAP-HSU:~/invenio-devbox$ ls
README.md  devbox.json  devbox.lock  devbox_scripts  invenio-test  my-site
garyhsu@G05-LAP-HSU:~/invenio-devbox$

6. IN





## Documentation Tools
### Read the docs

### Gitbook

### Collection
[https://github.com/MaggieAppleton/digital-gardeners](https://github.com/MaggieAppleton/digital-gardeners)

### HedgeDoc


## Online Diagram Plotting Tools
### Rawgraphs
https://app.rawgraphs.io/



