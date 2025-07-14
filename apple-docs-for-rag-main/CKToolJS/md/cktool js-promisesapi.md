

- CKTool JS
-  PromisesApi 

Class

# PromisesApi

A class that exposes promise-based functions for interacting with the API.

CKTool JS 1.2.15+

``` source
interface PromisesApi
```

## Mentioned in 

Integrating CloudKit access into your JavaScript automation scripts

## Overview

You use an instance of `PromisesApi` to interact with the API. Methods on this class return promises that complete with a response object.

## Topics

### Record Management

acceptRecord

Accepts a share on behalf of the current user.

createRecord

Creates a new record.

deleteRecord

Deletes a single record.

deleteRecordsByQuery

Deletes records matching the provided query.

getRecord

Returns a record’s details.

lookupRecords

Fetches multiple records by record name.

queryRecordChanges

Returns records that changed since a specified sync token or since a zone was created.

queryRecords

Returns a collection of records matching the provided query.

resolveRecord

Fetches information about records given their shortGuid properties.

updateRecord

Updates an existing record.

### Zone Management

createZone

Creates a new zone.

deleteZone

Deletes a zone.

getZone

Returns details for a zone.

getZones

Returns a collection of zones.

### Database Management

exportSchema

Downloads the container’s schema.

getContainers

Fetches containers for a team.

importSchema

Uploads a file that defines the new schema for the container.

resetConfigToProduction

Resets the container configuration to production.

resetToProduction

Resets the schema of the environment to production.

validateSchema

Validates the uploaded schema file for the container.

### Database Field Values, Structures and Enumerations

Field Values

Database Structures and Enumerations

### Asset Creation

createAssetUploadUrl

Creates a new URL for uploading assets.

### User and Team

getSessionUser

Returns details for the user in current session.

getTeams

Fetches a list of teams the current user is in.

Team

Details of a developer team.

TeamsResponse

Response object for a list of teams.

### Initialization

PromisesApi

Creates a `PromisesApi` object.

PromisesApiOptions

A dictionary of options for promises API classes.

Security

A dictionary of your authorization tokens.

## See Also

### Promises API

CancellablePromise

A promise that has a function to cancel its operation.

CKToolDatabaseModule

The imported package that provides access to CloudKit containers and databases.

