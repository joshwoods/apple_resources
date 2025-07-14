

- Core Foundation
-  CFErrorCreateWithUserInfoKeysAndValues(\_:\_:\_:\_:\_:\_:) 

Function

# CFErrorCreateWithUserInfoKeysAndValues(\_:\_:\_:\_:\_:\_:)

Creates a new CFError object using given keys and values to create the user info dictionary.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CFErrorCreateWithUserInfoKeysAndValues(
    _ allocator: CFAllocator!,
    _ domain: CFErrorDomain!,
    _ code: CFIndex,
    _ userInfoKeys: UnsafePointer!,
    _ userInfoValues: UnsafePointer!,
    _ numUserInfoValues: CFIndex
) -> CFError!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`domain`  

A CFString that identifies the error domain. If this reference is `NULL` or is otherwise not a valid CFString, the behavior is undefined.

`code`  

A CFIndex that identifies the error code. The code is interpreted within the context of the error domain.

`userInfoKeys`  

An array of `numUserInfoValues` CFStrings used as keys in creating the userInfo dictionary. The value of this parameter can be `NULL` if `numUserInfoValues` is `0`.

`userInfoValues`  

An array of `numUserInfoValues` CF types used as values in creating the userInfo dictionary. The value of this parameter can be `NULL` if `numUserInfoValues` is `0`.

`numUserInfoValues`  

The number of keys and values in the `userInfoKeys` and `userInfoValues` arrays.

## Return Value

A new CFError object. Ownership follows the The Create Rule.

## See Also

### Creating a CFError

func CFErrorCreate(CFAllocator!, CFErrorDomain!, CFIndex, CFDictionary!) -> CFError!

Creates a new CFError object.

