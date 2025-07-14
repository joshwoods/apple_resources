

- App Store Connect API
-  ScmProviderType 

Object

# ScmProviderType

The source code management provider’s type.

App Store Connect API 1.5+

``` source
object ScmProviderType
```

## Properties

`displayName`

`string`

The source code management provider’s display name; for example, `Bitbucket Server`.

`isOnPremise`

`boolean`

A Boolean value that indicates whether it’s a self-hosted source code management provider.

`kind`

`string`

A string that represents the kind of a Providers resource.

Possible Values: `BITBUCKET_CLOUD, BITBUCKET_SERVER, GITHUB_CLOUD, GITHUB_ENTERPRISE, GITLAB_CLOUD, GITLAB_SELF_MANAGED`

## See Also

### Objects and Types

object ScmProvider.Attributes

The attributes that describe a Providers resource.

