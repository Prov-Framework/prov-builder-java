# pro-builder-java

## Description
This is a non-executable jar with zero dependencies. The goal of this repo is to provide developers the Java classes they need to start building provenance objects and publishing Kafka for consumption by the prov-capture (https://github.com/Prov-Framework/prov-capture) repo. The prov capture repo uses this jar for deserializing JSON coming from Kafka, so using this jar or at least copying these classes into your code is the best way to ensure compatibility.

### PROV-O Concept Coverage
Provenance terms are broken into three categories (https://www.w3.org/TR/prov-o/#prov-o-at-a-glance):
1) Starting Point
2) Expanded
3) Qualified

Currently this library covers all of "Starting Point", plus "prov:Bundle", and "prov:atLocation" from the "Expanded" term list.

The supported concepts are listed below:

prov:Bundle   prov:Entity   prov:Activity   prov:Agent   prov:wasGeneratedBy   prov:wasDerivedFrom   prov:wasAttributedTo   prov:startedAtTime   prov:used   prov:wasInformedBy   prov:endedAtTime   prov:wasAssociatedWith  prov:actedOnBehalfOf   prov:atLocation

### TODO for 1.1.0 Release
- Add Expanded terms (in coordination with prov-capture support updates)