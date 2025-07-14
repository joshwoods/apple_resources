

- Security
-  SecAccessControlCreateWithFlags(\_:\_:\_:\_:) 

Function

# SecAccessControlCreateWithFlags(\_:\_:\_:\_:)

Creates a new access control object with the specified protection type and flags.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func SecAccessControlCreateWithFlags(
    _ allocator: CFAllocator?,
    _ protection: CFTypeRef,
    _ flags: SecAccessControlCreateFlags,
    _ error: UnsafeMutablePointer?>?
) -> SecAccessControl?
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new SecAccessControl object. Pass `NULL` or kCFAllocatorDefault to allocate memory for the new allocator using the default allocator.

`protection`  

Protection class to be used for the item. Use one of the values that go with the kSecAttrAccessible attribute key, namely those listed in Accessibility Values.

`flags`  

Flags specifying the allowed operations for the item. See SecAccessControlCreateFlags.

`error`  

On return, if an error occurred, the reference pointed at by this parameter refers to an error object that indicates the reason for failure. The caller is responsible for releasing the error object. Pass `NULL` for this parameter to ignore the error.

## Return Value

The newly created access control object. In Objective-C, free this item with CFRelease when you are done with it.

## Mentioned in 

Protecting keys with the Secure Enclave

Restricting keychain item accessibility

## Discussion

You use the result of this function as a value for the kSecAttrAccessControl attribute in the SecItemAdd(_:_:), SecItemUpdate(_:_:), or SecKeyGeneratePair(_:_:_:) functions.

Accessing keychain items or performing operations on keys that are protected by access control objects may block execution on the main thread. Perform these actions in the background, or use them in combination with the kSecUseAuthenticationContext and kSecUseAuthenticationUI attributes to manage user interactions.

