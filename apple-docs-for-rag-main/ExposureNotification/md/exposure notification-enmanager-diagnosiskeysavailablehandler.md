

- Exposure Notification
- ENManager
-  diagnosisKeysAvailableHandler 

Instance Property

# diagnosisKeysAvailableHandler

The handler that receives available diagnosis keys after a successful preauthorization.

iOS 14.4+iPadOS 14.4+Mac Catalyst 14.4+

``` source
var diagnosisKeysAvailableHandler: ENDiagnosisKeysAvailableHandler? { get set }
```

## Discussion

Set this property before calling requestPreAuthorizedDiagnosisKeys(completionHandler:) to ensure ENManager can deliver the keys. Authorization expires after five days or the first time this method is called after authorization, whichever comes first.

## See Also

### Preauthorizing Exposure Keys

func requestPreAuthorizedDiagnosisKeys(completionHandler: ENErrorHandler)

Requests diagnosis keys after the user authorizes sharing them.

func preAuthorizeDiagnosisKeys(completionHandler: ENErrorHandler)

Allows users to authorize a one-time release of diagnosis keys within five days of the authorization.

typealias ENDiagnosisKeysAvailableHandler

The handler the system invokes after requesting diagnosis keys.

