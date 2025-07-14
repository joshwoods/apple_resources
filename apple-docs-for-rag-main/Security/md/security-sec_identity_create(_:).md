

- Security
-  sec_identity_create(\_:) 

Function

# sec_identity_create(\_:)

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
func sec_identity_create(_ identity: SecIdentity) -> sec_identity_t?
```

## Parameters 

`identity`  

A `SecIdentityRef` instance.

## Return Value

A `sec_identity_t` instance.

## Discussion

```
  Create an ARC-able `sec_identity_t` instance from a `SecIdentityRef`.
```

