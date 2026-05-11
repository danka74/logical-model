# Current pregnancy obligations - EHDS Logical Information Models v0.1.0

## Logical Model: Current pregnancy obligations 

 
Obligations for the logical model for current pregnancy. 

**Usages:**

* This Logical Model Profile is not used by any profiles in this Implementation Guide

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/eu.ehds.models|current/StructureDefinition/EHDSCurrentPregnancyObligations)

### Formal Views of Profile Content

 [Description Differentials, Snapshots, and other representations](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](../StructureDefinition-EHDSCurrentPregnancyObligations.csv), [Excel](../StructureDefinition-EHDSCurrentPregnancyObligations.xlsx) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "EHDSCurrentPregnancyObligations",
  "url" : "http://ehds.eu/fhir/models/StructureDefinition/EHDSCurrentPregnancyObligations",
  "version" : "0.1.0",
  "name" : "EHDSCurrentPregnancyObligations",
  "title" : "Current pregnancy obligations",
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
  "description" : "Obligations for the logical model for current pregnancy.",
  "fhirVersion" : "5.0.0",
  "mapping" : [{
    "identity" : "rim",
    "uri" : "http://hl7.org/v3",
    "name" : "RIM Mapping"
  }],
  "kind" : "logical",
  "abstract" : false,
  "type" : "http://ehds.eu/fhir/models/StructureDefinition/EHDSCurrentPregnancy",
  "baseDefinition" : "http://ehds.eu/fhir/models/StructureDefinition/EHDSCurrentPregnancy",
  "derivation" : "constraint",
  "differential" : {
    "element" : [{
      "id" : "EHDSCurrentPregnancy",
      "path" : "EHDSCurrentPregnancy"
    },
    {
      "id" : "EHDSCurrentPregnancy.header",
      "extension" : [{
        "extension" : [{
          "url" : "code",
          "valueCode" : "SHALL:able-to-populate"
        },
        {
          "url" : "actor",
          "valueCanonical" : "https://www.xt-ehr.eu/specifications/fhir/actor-producer"
        }],
        "url" : "http://hl7.org/fhir/StructureDefinition/obligation"
      }],
      "path" : "EHDSCurrentPregnancy.header"
    },
    {
      "id" : "EHDSCurrentPregnancy.header.subject",
      "extension" : [{
        "extension" : [{
          "url" : "code",
          "valueCode" : "SHALL:able-to-populate"
        },
        {
          "url" : "actor",
          "valueCanonical" : "https://www.xt-ehr.eu/specifications/fhir/actor-producer"
        }],
        "url" : "http://hl7.org/fhir/StructureDefinition/obligation"
      }],
      "path" : "EHDSCurrentPregnancy.header.subject"
    },
    {
      "id" : "EHDSCurrentPregnancy.header.status",
      "extension" : [{
        "extension" : [{
          "url" : "code",
          "valueCode" : "SHALL:able-to-populate"
        },
        {
          "url" : "actor",
          "valueCanonical" : "https://www.xt-ehr.eu/specifications/fhir/actor-producer"
        }],
        "url" : "http://hl7.org/fhir/StructureDefinition/obligation"
      }],
      "path" : "EHDSCurrentPregnancy.header.status"
    },
    {
      "id" : "EHDSCurrentPregnancy.currentPregnancyStatus",
      "extension" : [{
        "extension" : [{
          "url" : "code",
          "valueCode" : "SHALL:able-to-populate"
        },
        {
          "url" : "actor",
          "valueCanonical" : "https://www.xt-ehr.eu/specifications/fhir/actor-producer"
        }],
        "url" : "http://hl7.org/fhir/StructureDefinition/obligation"
      }],
      "path" : "EHDSCurrentPregnancy.currentPregnancyStatus"
    },
    {
      "id" : "EHDSCurrentPregnancy.dateOfStatus",
      "extension" : [{
        "extension" : [{
          "url" : "code",
          "valueCode" : "SHALL:able-to-populate"
        },
        {
          "url" : "actor",
          "valueCanonical" : "https://www.xt-ehr.eu/specifications/fhir/actor-producer"
        }],
        "url" : "http://hl7.org/fhir/StructureDefinition/obligation"
      }],
      "path" : "EHDSCurrentPregnancy.dateOfStatus"
    },
    {
      "id" : "EHDSCurrentPregnancy.expectedDateOfDelivery",
      "extension" : [{
        "extension" : [{
          "url" : "code",
          "valueCode" : "SHALL:able-to-populate"
        },
        {
          "url" : "actor",
          "valueCanonical" : "https://www.xt-ehr.eu/specifications/fhir/actor-producer"
        }],
        "url" : "http://hl7.org/fhir/StructureDefinition/obligation"
      }],
      "path" : "EHDSCurrentPregnancy.expectedDateOfDelivery"
    }]
  }
}

```
