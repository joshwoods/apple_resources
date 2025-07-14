

- App Store Connect API
- CiArtifact
-  CiArtifact.Attributes 

Object

# CiArtifact.Attributes

The attributes that describe the output of an artifact resource.

App Store Connect API 1.5+

``` source
object CiArtifact.Attributes
```

## Properties

`downloadUrl`

`uri`

The URL you use to download the Xcode Cloud build artifact.

`fileName`

`string`

The artifact’s filename as a string.

`fileSize`

`integer`

An integer value that represents the artifact’s file size.

`fileType`

`string`

A string that describes the type of the artifact.

Possible Values: `ARCHIVE, ARCHIVE_EXPORT, LOG_BUNDLE, RESULT_BUNDLE, TEST_PRODUCTS, XCODEBUILD_PRODUCTS, STAPLED_NOTARIZED_ARCHIVE`

## Mentioned in 

App Store Connect API 3.2 release notes

