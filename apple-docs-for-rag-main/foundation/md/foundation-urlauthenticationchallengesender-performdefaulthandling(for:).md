

- Foundation
- URLAuthenticationChallengeSender
-  performDefaultHandling(for:) 

Instance Method

# performDefaultHandling(for:)

Causes the system-provided default behavior to be used.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func performDefaultHandling(for challenge: URLAuthenticationChallenge)
```

## Parameters 

`challenge`  

The challenge for which the default behavior should be used.

## See Also

### Protocol Methods

func cancel(URLAuthenticationChallenge)

Cancels a given authentication challenge.

**Required**

func continueWithoutCredential(for: URLAuthenticationChallenge)

Attempt to continue downloading a request without providing a credential for a given challenge.

**Required**

func use(URLCredential, for: URLAuthenticationChallenge)

Attempt to use a given credential for a given authentication challenge.

**Required**

func rejectProtectionSpaceAndContinue(with: URLAuthenticationChallenge)

Rejects the currently supplied protection space.

