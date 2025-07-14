

- App Store Connect API
- CiXcodeVersion
- CiXcodeVersion.Relationships
-  CiXcodeVersion.Relationships.MacOsVersions 

Object

# CiXcodeVersion.Relationships.MacOsVersions

The data, links, and paging information that describe the relationship between the Xcode Versions and the macOS Versions resources.

App Store Connect API 1.5+

``` source
object CiXcodeVersion.Relationships.MacOsVersions
```

## Properties

`data`

`[`CiXcodeVersion.Relationships.MacOsVersions.Data`]`

The ID and type of the related macOS Versions resource.

`links`

RelationshipLinks

The navigational links that include the self-link.

`meta`

PagingInformation

The paging information.

## Topics

### Objects

object CiXcodeVersion.Relationships.MacOsVersions.Data

The type and ID of a related macOS Versions resource.

