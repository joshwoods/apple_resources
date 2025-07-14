

- Security
-  SecKeyCopyAttributes(\_:) 

Function

# SecKeyCopyAttributes(\_:)

Gets the attributes of a given key.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func SecKeyCopyAttributes(_ key: SecKey) -> CFDictionary?
```

## Parameters 

`key`  

The key whose attributes you want.

## Return Value

A dictionary containing the key’s attributes. In Objective-C, call the CFRelease function to free this dictionary’s memory when you are done with it.

