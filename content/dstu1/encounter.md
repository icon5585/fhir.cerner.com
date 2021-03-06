---
title: Encounter | FHIR API
---

# Encounter

* TOC
{:toc}

## Search

Search for Encounters that meet supplied query parameters:

    GET /Encounter?:parameters

### Parameters

 Name            | Type                                                                           | Description
-----------------|--------------------------------------------------------------------------------|-------------------------------------------------------
`subject:Patient`|[`reference`](http://www.hl7.org/implement/standards/fhir/search.html#reference)| The patient present at the encounter. Example: `12345`

### Response

<%= headers 200 %>
<%= json(:dstu1_encounter_bundle) %>

## Retrieve by id

List an individual Encounter by its id:

    GET /Encounter/:id

### Response

<%= headers 200 %>
<%= json(:dstu1_encounter) %>