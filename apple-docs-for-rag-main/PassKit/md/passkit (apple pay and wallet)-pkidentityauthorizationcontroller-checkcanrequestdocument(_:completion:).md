

- PassKit (Apple Pay and Wallet)
- PKIdentityAuthorizationController
-  checkCanRequestDocument(\_:completion:) 

Instance Method

# checkCanRequestDocument(\_:completion:)

Returns whether an identity document is available to request.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
func checkCanRequestDocument(
    _ descriptor: any PKIdentityDocumentDescriptor,
    completion: @escaping (Bool) -> Void
)
```

``` source
func canRequestDocument(_ descriptor: any PKIdentityDocumentDescriptor) async -> Bool
```

## Parameters 

`descriptor`  

The object that describes the document the app requests.

`completion`  

The callback the system invokes after determining whether you can request the document you describe.

## Mentioned in 

Requesting identity data from a Wallet pass

## Discussion

This method checks whether you have the correct entitlements and if the device has an ID in the Wallet app.

```
// Check whether the app can request the document.
controller.checkCanRequestDocument(descriptor) { canRequest in
    if canRequest {
        // Show the identity button for triggering the request.
    } else {
        // Hide the request button.
    }
}
```

## See Also

### Requesting a document

func requestDocument(PKIdentityRequest, completion: (PKIdentityDocument?, (any Error)?) -> Void)

Prompts the user to approve the request to get the identity information.

