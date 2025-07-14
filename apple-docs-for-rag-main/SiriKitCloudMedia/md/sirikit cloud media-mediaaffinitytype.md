

- SiriKit Cloud Media
-  MediaAffinityType 

Type

# MediaAffinityType

A preference or dislike for a media item.

SiriKit Cloud Media 1.0.2+

``` source
string MediaAffinityType
```

## Possible Values 

`like`  

The user likes the media item.

`dislike`  

The user dislikes the media item.

`unknown`  

An unspecified preference.

## See Also

### Discerning Like or Dislike

object UpdateMediaAffinityIntentHandlingResolveAffinityTypeInvocationResponse

Your service’s response to a request that expresses a preference or dislike for a media item.

object MediaAffinityTypeResolutionResult

A media affinity that matches an update media affinity intent, or information about why your service can’t determine the media affinity.

