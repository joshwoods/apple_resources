

- Foundation
- URLAuthenticationChallengeSender
-  use(\_:for:) 

Instance Method

# use(\_:for:)

Attempt to use a given credential for a given authentication challenge.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func use(
    _ credential: URLCredential,
    for challenge: URLAuthenticationChallenge
)
```

**Required**

## Parameters 

`credential`  

The credential to use for authentication.

`challenge`  

The challenge for which to use `credential`.

## Discussion

This method has no effect if it is called with an authentication challenge that has already been handled.

## See Also

### Protocol Methods

func cancel(URLAuthenticationChallenge)

Cancels a given authentication challenge.

**Required**

func continueWithoutCredential(for: URLAuthenticationChallenge)

Attempt to continue downloading a request without providing a credential for a given challenge.

**Required**

func performDefaultHandling(for: URLAuthenticationChallenge)

Causes the system-provided default behavior to be used.

func rejectProtectionSpaceAndContinue(with: URLAuthenticationChallenge)

Rejects the currently supplied protection space.

