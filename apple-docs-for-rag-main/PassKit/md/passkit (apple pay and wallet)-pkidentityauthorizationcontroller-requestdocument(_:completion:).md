

- PassKit (Apple Pay and Wallet)
- PKIdentityAuthorizationController
-  requestDocument(\_:completion:) 

Instance Method

# requestDocument(\_:completion:)

Prompts the user to approve the request to get the identity information.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
func requestDocument(
    _ request: PKIdentityRequest,
    completion: @escaping (PKIdentityDocument?, (any Error)?) -> Void
)
```

``` source
func requestDocument(_ request: PKIdentityRequest) async throws -> PKIdentityDocument
```

## Parameters 

`request`  

The object that contains the identity elements the app requests.

`completion`  

The callback the system invokes after retrieving the document, or an error if one occurs.

## Discussion

The user needs to approve the request before releasing any data. When the user approves the request, the system returns the document. If the user doesn’t approve the request, the handler returns a PKIdentityError.Code.cancelled error.

Only one request can be in progress at a time; otherwise, the method returns a PKIdentityError.Code.requestAlreadyInProgress error.

Your app’s `Info.plist` file needs to provide a message for the `NSIdentityUsageDescription` key. If this key is missing, any attempt to request a document fails.

## See Also

### Requesting a document

func checkCanRequestDocument(any PKIdentityDocumentDescriptor, completion: (Bool) -> Void)

Returns whether an identity document is available to request.

