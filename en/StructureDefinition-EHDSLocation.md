# Location model - EHDS Logical Information Models v0.1.0

## Logical Model: Location model 

 
Model for details and position information for a place where services are provided and resources and participants may be stored, found, contained, or accommodated. 

**Usages:**

* Use this Logical Model: [Encounter model](StructureDefinition-EHDSEncounter.md), [Medication dispense model](StructureDefinition-EHDSMedicationDispense.md), [Observation model](StructureDefinition-EHDSObservation.md) and [Specimen model](StructureDefinition-EHDSSpecimen.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/eu.ehds.models|current/StructureDefinition/EHDSLocation)

### Formal Views of Profile Content

 [Description Differentials, Snapshots, and other representations](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](../StructureDefinition-EHDSLocation.csv), [Excel](../StructureDefinition-EHDSLocation.xlsx) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "EHDSLocation",
  "url" : "http://ehds.eu/fhir/models/StructureDefinition/EHDSLocation",
  "version" : "0.1.0",
  "name" : "EHDSLocation",
  "title" : "Location model",
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
  "description" : "Model for details and position information for a place where services are provided and resources and participants may be stored, found, contained, or accommodated.",
  "fhirVersion" : "5.0.0",
  "mapping" : [{
    "identity" : "rim",
    "uri" : "http://hl7.org/v3",
    "name" : "RIM Mapping"
  }],
  "kind" : "logical",
  "abstract" : false,
  "type" : "http://ehds.eu/fhir/models/StructureDefinition/EHDSLocation",
  "baseDefinition" : "http://hl7.org/fhir/StructureDefinition/Base",
  "derivation" : "specialization",
  "differential" : {
    "element" : [{
      "id" : "EHDSLocation",
      "path" : "EHDSLocation",
      "short" : "Location model",
      "definition" : "Model for details and position information for a place where services are provided and resources and participants may be stored, found, contained, or accommodated."
    },
    {
      "id" : "EHDSLocation.identifier",
      "path" : "EHDSLocation.identifier",
      "short" : "Location identifier",
      "definition" : "Location identifier",
      "min" : 0,
      "max" : "*",
      "type" : [{
        "code" : "Identifier"
      }]
    },
    {
      "id" : "EHDSLocation.name",
      "path" : "EHDSLocation.name",
      "short" : "Name of the location as used by humans",
      "definition" : "Name of the location as used by humans",
      "min" : 0,
      "max" : "1",
      "type" : [{
        "code" : "string"
      }]
    },
    {
      "id" : "EHDSLocation.description",
      "path" : "EHDSLocation.description",
      "short" : "Additional details about the location that could be displayed as further information to identify the location beyond its name",
      "definition" : "Additional details about the location that could be displayed as further information to identify the location beyond its name",
      "min" : 0,
      "max" : "1",
      "type" : [{
        "code" : "string"
      }]
    },
    {
      "id" : "EHDSLocation.type",
      "path" : "EHDSLocation.type",
      "short" : "Type of function performed at the location",
      "definition" : "Type of function performed at the location",
      "min" : 0,
      "max" : "*",
      "type" : [{
        "code" : "CodeableConcept"
      }],
      "binding" : {
        "strength" : "preferred",
        "description" : "HL7 ServiceDeliveryLocationRoleType"
      }
    },
    {
      "id" : "EHDSLocation.address",
      "path" : "EHDSLocation.address",
      "short" : "Physical location address",
      "definition" : "Physical location address",
      "min" : 0,
      "max" : "1",
      "type" : [{
        "code" : "http://ehds.eu/fhir/models/StructureDefinition/EHDSAddress"
      }]
    },
    {
      "id" : "EHDSLocation.managingOrganisation",
      "path" : "EHDSLocation.managingOrganisation",
      "short" : "The organisation responsible for the provisioning and upkeep of the location",
      "definition" : "The organisation responsible for the provisioning and upkeep of the location",
      "min" : 0,
      "max" : "1",
      "type" : [{
        "code" : "http://ehds.eu/fhir/models/StructureDefinition/EHDSOrganisation"
      }]
    },
    {
      "id" : "EHDSLocation.partOf",
      "path" : "EHDSLocation.partOf",
      "short" : "Another location of which this location is physically a part of",
      "definition" : "Another location of which this location is physically a part of",
      "min" : 0,
      "max" : "1",
      "type" : [{
        "code" : "http://ehds.eu/fhir/models/StructureDefinition/EHDSOrganisation"
      }]
    }]
  }
}

```
