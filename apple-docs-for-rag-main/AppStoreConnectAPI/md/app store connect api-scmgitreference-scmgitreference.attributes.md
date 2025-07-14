

- App Store Connect API
- ScmGitReference
-  ScmGitReference.Attributes 

Object

# ScmGitReference.Attributes

The attributes that describe a Git Reference resource.

App Store Connect API 1.5+

``` source
object ScmGitReference.Attributes
```

## Properties

`canonicalName`

`string`

The canonical name of the Git reference.

`isDeleted`

`boolean`

A Boolean value that indicates whether the Git reference was deleted.

`kind`

CiGitRefKind

A value that indicates whether the Git reference is a tag or a branch.

`name`

`string`

The name of the Git reference.

## See Also

### Objects and Types

object ScmGitReference.Relationships

The relationships of the Git References resource you included in the request and those on which you can operate.

type CiGitRefKind

A string that represents the kind of a Git References resource.

