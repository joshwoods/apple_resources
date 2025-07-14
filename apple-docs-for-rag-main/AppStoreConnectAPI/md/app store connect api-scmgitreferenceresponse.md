

- App Store Connect API
-  ScmGitReferenceResponse 

Object

# ScmGitReferenceResponse

A response that contains a single Git References resource.

App Store Connect API 1.5+

``` source
object ScmGitReferenceResponse
```

## Properties

`data`

ScmGitReference

 (Required) 

The resource data.

`included`

`[`ScmRepository`]`

The requested relationship data.

`links`

DocumentLinks

 (Required) 

The navigational links that include the self-link.

## See Also

### Objects

object ScmGitReference

The data structure that represents a Git References resource.

object ScmGitReferencesResponse

A response that contains a list of Git References resources.

