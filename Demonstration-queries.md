This resource can be mined for interesting knowledge. Below are some examples, click on a question to run it in YASGUI:

### [What regimens include Declopramide?](http://yasgui.org/short/rkjAQkUYW)
```sparql
prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#>
prefix Declopramide: <http://purl.obolibrary.org/obo/NCIT_C1772>
prefix ChemotherapyRegimenHasComponent: <http://purl.obolibrary.org/obo/NCIT_R123>
select distinct ?regimen ?regimen_label where {
# ?s rdfs:label "Chemotherapy_Regimen_Has_Component"
?regimen rdfs:subClassOf* /ChemotherapyRegimenHasComponent: Declopramide: .
?regimen rdfs:label ?regimen_label .
}
```
