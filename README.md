# Firely.FhirMapper.Examples

<img src="https://fire.ly/wp-content/uploads/2019/12/Icon_FHIR_Mapper_Plugin-01.svg" width="200" height="200" />

The FHIR Mapper is an implementation of the [FHIR mapping language](https://www.hl7.org/fhir/mapping-language.html), developed by [Firely](https://fire.ly) and [Healex](https://healex.systems), available as a Vonk plugin on the [Vonk marketplace](https://fire.ly/products/vonk/plugins/). With this add-on you're able to transform data from a variety of formats - HL7 v2 or your custom ones - to other formats such as FHIR/custom resources. It can even be used to map FHIR resources between different profiles and FHIR versions.

More general information and tutorials about the FHIR Mapping Language can be found on the [HL7 wiki](https://confluence.hl7.org/display/FHIR/Using+the+FHIR+Mapping+Language).

This repository contains different branches, each containing StructureMaps and StructureDefintions defined for a certain use case / file format supported by the FHIR Mapper:

* HL7 FHIR Mapping Language Tutorial
* Firely FHIR Mapping Language Introduction
  - [FakeInpatientDrugChart Mapping (FHIR R4)](https://github.com/FirelyTeam/Firely.FhirMapper.Examples/tree/FakeInpatientDrugChart-R4)
  - [FakeInpatientDrugChart Mapping (FHIR STU3)](https://github.com/FirelyTeam/Firely.FhirMapper.Examples/tree/FakeInpatientDrugChart-STU3)
* CSV
* (C)-CDA to FHIR
  - [(C)-CDA Mapping (FHIR R4)](https://github.com/FirelyTeam/Firely.FhirMapper.Examples/tree/CCDA-R4)
  - [(C)-CDA Mapping (FHIR STU3)](https://github.com/FirelyTeam/Firely.FhirMapper.Examples/tree/CCDA-STU3)
* HL7 v2 to FHIR
* FHIR to FHIR
* VCF (Variant Call Format)

Examples on how transform the above-mentioned data formats can be found in the following Postman collection:

[![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/3a27666e366c56707949#?env%5BVonk%20Remote%20Firely%5D=W3sia2V5IjoiQkFTRV9VUkwiLCJ2YWx1ZSI6Imh0dHBzOi8vdm9uay5maXJlLmx5IiwiZW5hYmxlZCI6dHJ1ZX1d)
