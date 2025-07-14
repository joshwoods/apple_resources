

- SiriKit Cloud Media
- ExtensionConfig
- ExtensionConfig.Intent
-  ExtensionConfig.Intent.UpdateMediaAffinity 

Object

# ExtensionConfig.Intent.UpdateMediaAffinity

Configuration details for your service’s update media affinity intent.

SiriKit Cloud Media 1.0.2+

``` source
object ExtensionConfig.Intent.UpdateMediaAffinity
```

## Properties

`opt`

`[string]`

Optional intent-handling steps that updateMediaAffinity supports.

Value: `resolveAffinityType`

## Discussion

To specify that your service only implements the required methods, provide an empty array for the `opt` property. You may omit the `opt` property if your service implements all of the optional methods.

## Relationships

### Inherits From

- ExtensionEndpointConfig

## See Also

### Specifying Required Headers and Supported Processing for Each Intent

object ExtensionConfig.Intent.AddMedia

Configuration details for your service’s add media intent.

object ExtensionConfig.Intent.PlayMedia

Configuration details for your service’s play media intent.

