

- App Store Connect API
-  CiArtifact 

Object

# CiArtifact

The data structure that represents the output of an Xcode Cloud build action resource.

App Store Connect API 1.5+

``` source
object CiArtifact
```

## Properties

`attributes`

CiArtifact.Attributes

The attributes that describe the Artifacts resource.

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies an Artifacts resource.

`links`

ResourceLinks

The navigational links that include the self-link.

`type`

`string`

 (Required) 

The resource type.

Value: `ciArtifacts`

## Topics

### Objects

object CiArtifact.Attributes

The attributes that describe the output of an artifact resource.

## See Also

### Objects

object CiArtifactResponse

A response that contains a single Artifacts resource.

