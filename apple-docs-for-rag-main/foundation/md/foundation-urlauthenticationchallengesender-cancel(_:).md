

- Foundation
- URLAuthenticationChallengeSender
-  cancel(\_:) 

Instance Method

# cancel(\_:)

Cancels a given authentication challenge.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func cancel(_ challenge: URLAuthenticationChallenge)
```

**Required**

## Parameters 

`challenge`  

The authentication challenge to cancel.

## See Also

### Related Documentation

URL Loading System

Interact with URLs and communicate with servers using standard Internet protocols.

### Protocol Methods

func continueWithoutCredential(for: URLAuthenticationChallenge)

Attempt to continue downloading a request without providing a credential for a given challenge.

**Required**

func use(URLCredential, for: URLAuthenticationChallenge)

Attempt to use a given credential for a given authentication challenge.

**Required**

func performDefaultHandling(for: URLAuthenticationChallenge)

Causes the system-provided default behavior to be used.

func rejectProtectionSpaceAndContinue(with: URLAuthenticationChallenge)

Rejects the currently supplied protection space.

