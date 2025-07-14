

- Security
-  SecPolicyCreateRevocation(\_:) 

Function

# SecPolicyCreateRevocation(\_:)

Returns a policy object for checking revocation of certificates.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func SecPolicyCreateRevocation(_ revocationFlags: CFOptionFlags) -> SecPolicy?
```

## Parameters 

`revocationFlags`  

Flags that specify revocation checking options. See Revocation Policy Constants for a list of possible values.

## Return Value

A policy object or `nil` on failure.

## Discussion

It’s usually not necessary to create a revocation policy yourself unless you wish to override default system behavior, for example to force a particular method, or to disable revocation checking entirely.

