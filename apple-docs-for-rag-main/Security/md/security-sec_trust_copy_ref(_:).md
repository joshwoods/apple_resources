

- Security
-  sec_trust_copy_ref(\_:) 

Function

# sec_trust_copy_ref(\_:)

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
func sec_trust_copy_ref(_ trust: sec_trust_t) -> Unmanaged
```

## Parameters 

`trust`  

A `sec_trust_t` instance.

## Return Value

The underlying `SecTrustRef` instance.

## Discussion

```
  Copy a retained reference to the underlying `SecTrustRef` instance.
```

