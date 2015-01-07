# OpenBIM Benchmark

This benchmark includes a model validation and transformation use cases in the context of  construction industry.
It comes also with a set of EMF-compliant BIM (Building Information Model) models with increasing size going up to 1 Gb.
A BIM model is described using the IFC (Industry Foundation Classes) specification, a freely available format to describe, exchange,
and share information typically used within the building and facility management industry sector.
Input models are made publicly available [here](https://drive.google.com/file/d/0B-PgPQN6HURHTmlOVTVrWG92c28/view?usp=sharing)
## Use cases description

### Well formedness rules
This benchmark involves validating the set of well-formedness [rules]() over a given model, model that conforms to the IFC Ecore metamodel
(1). An Ecore metamodel is provided, coming from the open-source [BIMServer](https://github.com/opensourceBIM/BIMserver) project. The well-formedness rules are given in EXPRESS format and are meant to be translated to the query technology under evaluation.

### IFC2BIMXML
This benchmark involves performing the translation of a full IFC model into the BIMXML format.
Ecore metamodels for the source and target models are provided.
