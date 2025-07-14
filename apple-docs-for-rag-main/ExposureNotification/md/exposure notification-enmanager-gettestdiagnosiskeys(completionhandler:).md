

- Exposure Notification
- ENManager
-  getTestDiagnosisKeys(completionHandler:) 

Instance Method

# getTestDiagnosisKeys(completionHandler:)

Requests the temporary exposure keys, including the current key, used by this device for testing.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
func getTestDiagnosisKeys(completionHandler: @escaping ENGetDiagnosisKeysHandler)
```

``` source
func testDiagnosisKeys() async throws -> [ENTemporaryExposureKey]
```

## Parameters 

`completionHandler`  

The completion handler that the framework calls when the method completes.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func testDiagnosisKeys() async throws -> [ENTemporaryExposureKey]
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Important

This method is available in iOS 12.5, and in iOS 13.5 and later.

Every time this method is called, the framework will request the user to authorize the action.

Warning

This method is only for developers while testing, and requires a special entitlement that is not allowed in the App Store. It’s only intended for testing without needing to wait 24 hours for a key to be released.

## See Also

### Obtaining Exposure Keys

func getDiagnosisKeys(completionHandler: ENGetDiagnosisKeysHandler)

Requests the temporary exposure keys from the user’s device to share with a server.

class ENTemporaryExposureKey

The key used to generate rolling proximity identifiers.

