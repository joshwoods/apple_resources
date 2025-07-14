

- Security
-  SecPolicyCopyProperties(\_:) 

Function

# SecPolicyCopyProperties(\_:)

Returns a dictionary containing a policy’s properties.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func SecPolicyCopyProperties(_ policyRef: SecPolicy) -> CFDictionary?
```

## Parameters 

`policyRef`  

The policy from which properties should be copied.

## Return Value

A dictionary with the policy’s properties. See Security Policy Keys for a list of valid keys. In Objective-C, call the CFRelease function to free the dictionary’s memory when you are done with it.

