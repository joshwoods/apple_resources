

- Security
-  sec_trust_create(\_:) 

Function

# sec_trust_create(\_:)

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
func sec_trust_create(_ trust: SecTrust) -> sec_trust_t?
```

## Parameters 

`trust`  

A `SecTrustRef` instance.

## Return Value

A `sec_trust_t` instance.

## Discussion

```
  Create an ARC-able `sec_trust_t` instance from a `SecTrustRef`.
```

