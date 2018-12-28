# starfish
Open source web-based SKOS +AMT keyword publishing tool

## idea

* simple SKOS (ConceptScheme + Concept)
* relations with AMT just broader/narrower match related
* role chain axioms
  * (A)-[broader,p]->(B)-[broader,q]->(C) => (A)-[broader,p*q]->(C)
  * (A)-[narrower,p]->(B)-[narrower,q]->(C) => (A)-[narrower,p*q]->(C)
  * (A)-[match,p]->(B)-[match,q]->(C) => (A)-[match,p*q]->(C)
  * (A)-[related,p]->(B)-[related,q]->(C) => (A)-[related,p*q]->(C)
