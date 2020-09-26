## (C)-CDA (R4)

This project holds logical models, maps, and examples used to transform (C)-CDA documents to FHIR.

Content:
- Examples: CDA documents which can be used for testing of the (C)-CDA to FHIR transformation. It also contains the expected transformation targets in the form of FHIR bundles.
- StructureDefinition: StructureDefinitions for FHIR R4 representing a (C)-CDA documents and its corresponding data types. 
- Mappings: FHIR Mapping Language files and StructureMap resources representing the mapping between (C)-CDA and FHIR. Additionally, a ConceptMap is included documenting which (C)-CDA elements can be mapped to FHIR.

The documentation of the how to execute these mappings with the Firely FHIR Mapper can be found [here](http://docs.simplifier.net/mappingengine/index.html).

---

## Customization

- All logical models which were derived from "http://hl7.org/fhir/StructureDefiniton/Base" have been changed to derive from "http://hl7.org/fhir/StructureDefiniton/Element". "http://hl7.org/fhir/StructureDefiniton/Base" is only available in FHIR R5.
- The `ANY` datatype contains an extra element "type". The .NET API does not recongnize the xsi:type as a special element, therefore we need to provide type information for it.
- ClinicalDocument.effectiveTime is represented as a string instead of using the "TS" datatype. The TS.value element can't currently be selected in the .NET FHIRPath implementation.
- SXCM_TS, SXPR_TS, PIVL_TS, IVL_TS, EIVL-TS, IVL_INT, INT_POS, RTO-PQ-PQ, IVL-PQ contain a `_` in StructureDefinition.type instead of a `-`. All references to these datatpyes have been adjusted.
- The following datatypes contain an explicit .value element needed to select the primitive element value in the .NET API:
  * TS
  * ON
  * EN
  * ED
  * ST
