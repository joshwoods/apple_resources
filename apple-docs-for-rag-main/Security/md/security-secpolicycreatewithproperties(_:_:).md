

- Security
-  SecPolicyCreateWithProperties(\_:\_:) 

Function

# SecPolicyCreateWithProperties(\_:\_:)

Returns a policy object based on an object identifier for the policy type.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func SecPolicyCreateWithProperties(
    _ policyIdentifier: CFTypeRef,
    _ properties: CFDictionary?
) -> SecPolicy?
```

## Parameters 

`policyIdentifier`  

The identifier for the desired policy type.

`properties`  

A properties dictionary. See Security Policy Keys for a list of valid property names to use as keys in this dictionary.

## Return Value

A new policy, or `NULL` if the policy could not be created.

## Mentioned in 

Creating a Trust Object

