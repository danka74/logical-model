# Travel history model - EHDS Logical Information Models v0.1.0

## Logical Model: Travel history model 

 
Relevant information about the patient's recent travel history, for one visit 

**Usages:**

* Use this Logical Model: [Patient summary model](StructureDefinition-EHDSPatientSummary.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/eu.ehds.models|current/StructureDefinition/EHDSTravelHistory)

### Formal Views of Profile Content

 [Description Differentials, Snapshots, and other representations](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](../StructureDefinition-EHDSTravelHistory.csv), [Excel](../StructureDefinition-EHDSTravelHistory.xlsx) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "EHDSTravelHistory",
  "url" : "http://ehds.eu/fhir/models/StructureDefinition/EHDSTravelHistory",
  "version" : "0.1.0",
  "name" : "EHDSTravelHistory",
  "title" : "Travel history model",
  "status" : "draft",
  "date" : "2026-05-11T13:28:07+00:00",
  "publisher" : "EC",
  "contact" : [{
    "name" : "EC",
    "telecom" : [{
      "system" : "url",
      "value" : "http://commission.europa.eu/"
    }]
  }],
  "description" : "Relevant information about the patient's recent travel history, for one visit",
  "fhirVersion" : "5.0.0",
  "mapping" : [{
    "identity" : "rim",
    "uri" : "http://hl7.org/v3",
    "name" : "RIM Mapping"
  }],
  "kind" : "logical",
  "abstract" : false,
  "type" : "http://ehds.eu/fhir/models/StructureDefinition/EHDSTravelHistory",
  "baseDefinition" : "http://ehds.eu/fhir/models/StructureDefinition/EHDSDataSet",
  "derivation" : "specialization",
  "differential" : {
    "element" : [{
      "id" : "EHDSTravelHistory",
      "path" : "EHDSTravelHistory",
      "short" : "Travel history model",
      "definition" : "Relevant information about the patient's recent travel history, for one visit"
    },
    {
      "id" : "EHDSTravelHistory.country",
      "path" : "EHDSTravelHistory.country",
      "short" : "Country visited",
      "definition" : "Country visited",
      "requirements" : "eHN PS Guideline",
      "min" : 1,
      "max" : "1",
      "type" : [{
        "code" : "CodeableConcept"
      }],
      "binding" : {
        "strength" : "preferred",
        "description" : "ISO 3166"
      }
    },
    {
      "id" : "EHDSTravelHistory.period",
      "path" : "EHDSTravelHistory.period",
      "short" : "Date of entry and departure",
      "definition" : "The period during which the patient visited the country",
      "requirements" : "eHN PS Guideline",
      "min" : 0,
      "max" : "1",
      "type" : [{
        "code" : "Period"
      }]
    }]
  }
}

```
