

- Security
-  SecIdentityCopyPrivateKey(\_:\_:) 

Function

# SecIdentityCopyPrivateKey(\_:\_:)

Retrieves the private key associated with an identity.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.3+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func SecIdentityCopyPrivateKey(
    _ identityRef: SecIdentity,
    _ privateKeyRef: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`identityRef`  

The identity object for the identity whose private key you wish to retrieve.

`privateKeyRef`  

On return, points to the private key object for the specified identity. The private key must be of class type SecItemClass.privateKeyItemClass. In Objective-C, call the CFRelease function to release this object when you are finished with it.

## Return Value

A result code. See Security Framework Result Codes.

## Mentioned in 

Parsing an Identity

## Discussion

An identity is a digital certificate together with its associated private key.

