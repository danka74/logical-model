# Organisation obligations - EHDS Logical Information Models v0.1.0

## Logical Model: Organisation obligations 

 
Obligations for the logical model for organisation. 

**Usages:**

* This Logical Model Profile is not used by any profiles in this Implementation Guide

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/eu.ehds.models|current/StructureDefinition/EHDSOrganisationObligations)

### Formal Views of Profile Content

 [Description Differentials, Snapshots, and other representations](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](../StructureDefinition-EHDSOrganisationObligations.csv), [Excel](../StructureDefinition-EHDSOrganisationObligations.xlsx) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "EHDSOrganisationObligations",
  "url" : "http://ehds.eu/fhir/models/StructureDefinition/EHDSOrganisationObligations",
  "version" : "0.1.0",
  "name" : "EHDSOrganisationObligations",
  "title" : "Organisation obligations",
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
  "description" : "Obligations for the logical model for organisation.",
  "fhirVersion" : "5.0.0",
  "mapping" : [{
    "identity" : "rim",
    "uri" : "http://hl7.org/v3",
    "name" : "RIM Mapping"
  }],
  "kind" : "logical",
  "abstract" : false,
  "type" : "http://ehds.eu/fhir/models/StructureDefinition/EHDSOrganisation",
  "baseDefinition" : "http://ehds.eu/fhir/models/StructureDefinition/EHDSOrganisation",
  "derivation" : "constraint",
  "differential" : {
    "element" : [{
      "id" : "EHDSOrganisation",
      "path" : "EHDSOrganisation"
    },
    {
      "id" : "EHDSOrganisation.identifier",
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
      "path" : "EHDSOrganisation.identifier"
    },
    {
      "id" : "EHDSOrganisation.name",
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
      "path" : "EHDSOrganisation.name"
    },
    {
      "id" : "EHDSOrganisation.telecom",
      "extension" : [{
        "extension" : [{
          "url" : "code",
          "valueCode" : "SHOULD:able-to-populate"
        },
        {
          "url" : "actor",
          "valueCanonical" : "https://www.xt-ehr.eu/specifications/fhir/actor-producer"
        }],
        "url" : "http://hl7.org/fhir/StructureDefinition/obligation"
      }],
      "path" : "EHDSOrganisation.telecom"
    }]
  }
}

```
