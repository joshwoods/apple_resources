

- StoreKit
- AppTransaction
-  refresh() 

Type Method

# refresh()

Gets the App Store-signed app transaction information from the App Store server.

iOS 16.0+iPadOS 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func refresh() async throws -> VerificationResult
```

## Return Value

Returns a VerificationResult with a single AppTransaction.

## Discussion

This method queries the App Store server to refresh the app transaction information. This method returns a VerificationResult that contains the App Store-signed app transaction information for your app.

Important

Calling refresh() displays a system prompt that asks users to authenticate with their App Store credentials. Call this function only in response to an explicit user action, like tapping or clicking a button.

Use this method to get an AppTransaction in the following cases:

- The shared property throws an error.

- The shared property returns an unverified (VerificationResult.unverified(_:_:) ) result.

This method throws an error if the user cancels the authentication prompt, if there’s no network connectivity, or if the call fails to update the app transaction.

