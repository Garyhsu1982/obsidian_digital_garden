---
{"dg-publish":true,"permalink":"/nfdi-4-objects/tools-and-resouces/knowledge-graph/","noteIcon":""}
---

## Wikidata

- Wikidata Workshop at the University of Münster [presentation](https://pad.otc.coscine.dev/2025-04-01_wikidata-workshop)

Example SPARQL code
``` 
#defaultView:Map
SELECT ?consoritum ?consoritumLabel ?affiliation ?affiliationLabel ?geo
WHERE
{
  ?consoritum wdt:P361 wd:Q61658497.
 
  ?consoritum wdt:P31 wd:Q98270496.
  
  ?consoritum wdt:P1416 ?affiliation.
  
  OPTIONAL {?affiliation wdt:P625 ?geo.}
  
  SERVICE wikibase:label {bd:serviceParam wikibase:language "en".}
}
```

Corresponding Result (insert as HTML iframe)

<iframe style="width: 60vw; height: 50vh; border: none;" src="https://query.wikidata.org/embed.html#%23defaultView%3AMap%0ASELECT%20%3Fconsoritum%20%3FconsoritumLabel%20%3Faffiliation%20%3FaffiliationLabel%20%3Fgeo%0AWHERE%0A%7B%0A%20%20%3Fconsoritum%20wdt%3AP361%20wd%3AQ61658497.%0A%20%0A%20%20%3Fconsoritum%20wdt%3AP31%20wd%3AQ98270496.%0A%20%20%0A%20%20%3Fconsoritum%20wdt%3AP1416%20%3Faffiliation.%0A%20%20%0A%20%20OPTIONAL%20%7B%3Faffiliation%20wdt%3AP625%20%3Fgeo.%7D%0A%20%20%0A%20%20SERVICE%20wikibase%3Alabel%20%7Bbd%3AserviceParam%20wikibase%3Alanguage%20%22en%22.%7D%0A%7D%0A%20%20" referrerpolicy="origin" sandbox="allow-scripts allow-same-origin allow-popups"></iframe>


Example SPARQL code
``` 
SELECT ?consortium ?consortiumLabel (COUNT(DISTINCT ?affiliation) AS ?uniqueAffliaitions)
WHERE
{
  ?consortium wdt:P361 wd:Q61658497.
 
  ?consortium wdt:P31 wd:Q98270496.
  
  ?consortium wdt:P1416 ?affiliation.
  
  
  SERVICE wikibase:label {bd:serviceParam wikibase:language "en".}
}
GROUP BY ?consortium ?consortiumLabel
```

Corresponding Results (Table)
<iframe style="width: 60vw; height: 60vh; border: none;" src="https://query.wikidata.org/embed.html#SELECT%20%3Fconsortium%20%3FconsortiumLabel%20(COUNT(DISTINCT%20%3Faffiliation)%20AS%20%3FuniqueAffliaitions)%0AWHERE%0A%7B%0A%20%20%3Fconsortium%20wdt%3AP361%20wd%3AQ61658497.%0A%20%0A%20%20%3Fconsortium%20wdt%3AP31%20wd%3AQ98270496.%0A%20%20%0A%20%20%3Fconsortium%20wdt%3AP1416%20%3Faffiliation.%0A%20%20%0A%20%20%0A%20%20SERVICE%20wikibase%3Alabel%20%7Bbd%3AserviceParam%20wikibase%3Alanguage%20%22en%22.%7D%0A%7D%0AGROUP%20BY%20%3Fconsortium%20%3FconsortiumLabel" referrerpolicy="origin" sandbox="allow-scripts allow-same-origin allow-popups"></iframe>


## examples of LOD
FactGrid: [wikipage](https://database.factgrid.de/wiki/Main_Page), [SPARQL](https://database.factgrid.de/query/)
https://ogham.link/
https://rgzm.github.io/samian-lod/
https://romanopendata.eu/#!/
http://kerameikos.org/
https://numismatics.org/ocre/
https://nomisma.org/
NFDI4O KG https://graph.nfdi4objects.net/sparql
RDF star: https://www.w3.org/groups/wg/rdf-star/
Ariadne [graph database](https://graphdb.ariadne.d4science.org/) . [endpoint](https://graphdb.ariadne.d4science.org/repositories/ariadneplus-pr01)



