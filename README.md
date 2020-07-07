# Procurement units
## Description:

In Mexico, the Public Sector Acquisition, Leasing and Services Act defines three types of units who participate in the contracting processes: the Requesting Unit, the Contracting Unit and the Technical Unit.
Therefore, to align the Open Contracting Data Standard (OCDS) with transparency obligations in Mexico, we need to develop an extension that includes the classification of procurement units.
Considering the procurement units are known since planning stage, we propose to include them in the planning array.

## Proposal:

Add an array to the planning object. This array must contain the following attributes:

## Schema:

  - Planning {object}
    - contractingUnit {object}
      -  $ref: # /definitions/ OrganizationReference
    - requestingUnit {object}
      -  $ref: # /definitions/ OrganizationReference
    - technicalUnit {object}
      -  $ref: # /definitions/ OrganizationReference

## Party Roles

  - contractingUnit
  - requestingUunit
  - technicalUnit

## Defining texts:

**Code** | **Title** | **Description**
--|--|--
contractingUnit | Contracting unit | The authority in the agency or entity to carry out contracting procedures in order to acquire or lease goods or contract the provision of services required by the agency or entity in question.
requestingUnit | Requesting unit | The authority that in the agency or entity formally requests or requires the acquisition or lease of goods or the provision of services, or who will use them
technicalUnit | Technical unit | The authority in the agency or entity that prepares the technical specifications to be included in the contracting procedure, evaluates the technical proposal of the propositions and is responsible for answering the questions that the bidders ask about these aspects; The technical area may also have the character of the requesting area.
