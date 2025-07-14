

- Exposure Notification
- ENManager
-  getDiagnosisKeys(completionHandler:) 

Instance Method

# getDiagnosisKeys(completionHandler:)

Requests the temporary exposure keys from the user’s device to share with a server.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
func getDiagnosisKeys(completionHandler: @escaping ENGetDiagnosisKeysHandler)
```

``` source
func diagnosisKeys() async throws -> [ENTemporaryExposureKey]
```

## Parameters 

`completionHandler`  

The completion handler that the framework calls when getDiagnosisKeys(completionHandler:) completes. If the method completes successfully, `keys` will contain the diagnosis keys for this device and `error` will be `nil`. If it fails, `keys` will be `nil` and `error` indicates the reason it failed.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func diagnosisKeys() async throws -> [ENTemporaryExposureKey]
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Important

This method is available in iOS 12.5, and in iOS 13.5 and later.

The app must be in the foreground when it calls this method. Each time the app calls this method, the system presents an interface that requests authorization.

When ENAPIVersion is set to `1` in the app’s Info.plist file, you must wait approximately 24 hours after the first call of getDiagnosisKeys(completionHandler:) before this call returns a valid key. To test your app without waiting 24 hours, use getTestDiagnosisKeys(completionHandler:).

When ENAPIVersion is set to `2`, this call returns a diagnosis key with a shortened rolling period.

## Topics

### Completion Handlers

typealias ENGetDiagnosisKeysHandler

The definition of a handler that returns diagnosis keys.

## See Also

### Obtaining Exposure Keys

func getTestDiagnosisKeys(completionHandler: ENGetDiagnosisKeysHandler)

Requests the temporary exposure keys, including the current key, used by this device for testing.

class ENTemporaryExposureKey

The key used to generate rolling proximity identifiers.

