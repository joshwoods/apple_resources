

- Security
-  sec_identity_copy_ref(\_:) 

Function

# sec_identity_copy_ref(\_:)

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
func sec_identity_copy_ref(_ identity: sec_identity_t) -> Unmanaged?
```

## Parameters 

`identity`  

A `sec_identity_t` instance.

## Return Value

The underlying `SecIdentityRef` instance.

## Discussion

```
  Copy a retained reference to the underlying `SecIdentityRef` instance.
```

