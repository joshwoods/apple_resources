

- Exposure Notification
-  ENDiagnosisKeysAvailableHandler 

Type Alias

# ENDiagnosisKeysAvailableHandler

The handler the system invokes after requesting diagnosis keys.

iOS 14.4+iPadOS 14.4+Mac Catalyst 14.4+

``` source
typealias ENDiagnosisKeysAvailableHandler = ([ENTemporaryExposureKey]) -> Void
```

## Parameters 

`keys`  

An array of temporary exposure keys.

## See Also

### Preauthorizing Exposure Keys

func requestPreAuthorizedDiagnosisKeys(completionHandler: ENErrorHandler)

Requests diagnosis keys after the user authorizes sharing them.

func preAuthorizeDiagnosisKeys(completionHandler: ENErrorHandler)

Allows users to authorize a one-time release of diagnosis keys within five days of the authorization.

var diagnosisKeysAvailableHandler: ENDiagnosisKeysAvailableHandler?

The handler that receives available diagnosis keys after a successful preauthorization.

