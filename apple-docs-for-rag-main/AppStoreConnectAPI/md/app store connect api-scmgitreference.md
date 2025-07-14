

- App Store Connect API
-  ScmGitReference 

Object

# ScmGitReference

The data structure that represents a Git References resource.

App Store Connect API 1.5+

``` source
object ScmGitReference
```

## Properties

`attributes`

ScmGitReference.Attributes

The attributes that describe the Git References resource.

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies a Git References resource.

`links`

ResourceLinks

The navigational links that include the self-link.

`relationships`

ScmGitReference.Relationships

The navigational links to related data and included resource types and IDs.

`type`

`string`

 (Required) 

The resource type.

Value: `scmGitReferences`

## Topics

### Objects and Types

object ScmGitReference.Attributes

The attributes that describe a Git Reference resource.

object ScmGitReference.Relationships

The relationships of the Git References resource you included in the request and those on which you can operate.

type CiGitRefKind

A string that represents the kind of a Git References resource.

## See Also

### Objects

object ScmGitReferenceResponse

A response that contains a single Git References resource.

object ScmGitReferencesResponse

A response that contains a list of Git References resources.

