

- Security
-  SecPolicyCreateBasicX509() 

Function

# SecPolicyCreateBasicX509()

Returns a policy object for the default X.509 policy.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func SecPolicyCreateBasicX509() -> SecPolicy
```

## Return Value

The policy object. In Objective-C, call the CFRelease function to release the object when you are finished with it.

## Mentioned in 

Creating a Trust Object

