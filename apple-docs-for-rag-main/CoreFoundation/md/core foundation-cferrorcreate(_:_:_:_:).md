

- Core Foundation
-  CFErrorCreate(\_:\_:\_:\_:) 

Function

# CFErrorCreate(\_:\_:\_:\_:)

Creates a new CFError object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CFErrorCreate(
    _ allocator: CFAllocator!,
    _ domain: CFErrorDomain!,
    _ code: CFIndex,
    _ userInfo: CFDictionary!
) -> CFError!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`domain`  

A CFString that identifies the error domain. If this reference is `NULL` or is otherwise not a valid CFString, the behavior is undefined.

`code`  

A CFIndex that identifies the error code. The code is interpreted within the context of the error domain.

`userInfo`  

A CFDictionary created with kCFCopyStringDictionaryKeyCallBacks and kCFTypeDictionaryValueCallBacks. The dictionary is copied with CFDictionaryCreateCopy(_:_:). If you do not want the userInfo dictionary, you can pass `NULL`, in which case an empty dictionary will be assigned.

## Return Value

A new CFError object. Ownership follows the The Create Rule.

## See Also

### Creating a CFError

func CFErrorCreateWithUserInfoKeysAndValues(CFAllocator!, CFErrorDomain!, CFIndex, UnsafePointer&lt;UnsafeRawPointer?>!, UnsafePointer&lt;UnsafeRawPointer?>!, CFIndex) -> CFError!

Creates a new CFError object using given keys and values to create the user info dictionary.

