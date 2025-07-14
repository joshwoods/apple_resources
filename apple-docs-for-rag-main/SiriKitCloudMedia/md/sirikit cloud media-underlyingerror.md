

- SiriKit Cloud Media
-  UnderlyingError 

Object

# UnderlyingError

An object that describes a system framework error.

SiriKit Cloud Media 1.0.2+

``` source
object UnderlyingError
```

## Properties

`errorCode`

`int64`

 (Required) 

The error’s identity.

`errorDomain`

`string`

 (Required) 

The error’s domain.

Minimum length: `0`

Maximum length: `500`

## Discussion

The client depends on a number of system frameworks that manage user interaction and media playback, each of which can generate its own errors. For example, if your service provides a Content object that contains a malformed or expired URL, the AVFoundation framework generates an error when it attempts to load that URL. The client uses this object to provide details of the framework error when it reports the playback failure to your service. For more information, see Recover from Content Playback Failure.

An error code is unique only within its associated error domain. Therefore, use `errorDomain` to determine the origin of the error on the client, and then use `errorCode` to identify the specific error within that domain.

