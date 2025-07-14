

- Device Management
-  SeedBuildToken 

Object

# SeedBuildToken

Describes a beta enrollment token available for the given organization.

Device Assignment ServicesVPP License Management

``` source
object SeedBuildToken
```

## Properties

`os`

`string`

The platform related to beta build. Possible values are: `homePodOS`, `iOS`, `OSX`, `tvOS`, `visionOS`, `watchOS`\]

`title`

`string`

The public facing name, like “iOS 17 Public Beta”.

`token`

`string`

The token to use when requesting the beta build.

## See Also

### Response

object GetSeedBuildTokenResponse

Provides a list of beta enrollment tokens available for the given organization.

