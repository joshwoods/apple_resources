

- Security
-  SecCodeCopyGuestWithAttributes(\_:\_:\_:\_:) 

Function

# SecCodeCopyGuestWithAttributes(\_:\_:\_:\_:)

Asks a code host to identify one of its guests given the type and value of specific attributes of the guest code.

macOS 10.0+

``` source
func SecCodeCopyGuestWithAttributes(
    _ host: SecCode?,
    _ attributes: CFDictionary?,
    _ flags: SecCSFlags,
    _ guest: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`host`  

A valid code object representing code running on the system that acts as a host for signed code. Pass `NULL` to indicate that the code signing root of trust (currently, the system kernel) should be used as the code host.

`attributes`  

A dictionary containing zero or more attribute values to be used in identifying guest code. See Guest Attribute Dictionary Keys for possible dictionary keys and descriptions of the associated values. Each host supports only particular combinations of keys and values, and the function returns an error if any unsupported set is requested. Pass `NULL` to indicate an empty attribute set. Note that some hosts that support hosting chains (guests being hosts) may return sub-guests to this function; that is, the code object returned by this call may not be a direct guest of the queried host, although it will be a guest somewhere in the hosting chain.

`flags`  

Optional flags; see SecCSFlags for possible values. Pass kSecCSDefaultFlags for standard behavior.

`guest`  

On return, a code object identifying the particular guest of the host that has the specified attribute values. If the attributes specify the host itself, the function returns the code object for the host. If more than one guest meet the specified criteria, the function returns the result `errSecCSMultipleGuests`.

## Return Value

A result code. See Code Signing Services Result Codes. In particular:

errSecCSUnsupportedGuestAttributes  
The host does not support the specified attribute type.

errSecCSInvalidAttributeValues  
The type of value given for a guest attribute is not supported by the host.

errSecCSNoSuchCode  
The host has no guest with the specified attribute value, even though the value is of a supported type. This error may also be returned if the code specified in the `host` parameter is not currently acting as a code host.

errSecCSNotAHost  
The code specified in the `host` parameter cannot act as a code host, because it’s missing the host option flag in its code signature.

errSecCSMultipleGuests  
The attributes specified do not unambiguously identify a guest (the specification is not unique).

## Discussion

Different hosts support different types and combinations of attributes. The methods a host uses to identify, separate, and control its guests are specific to each type of host. This function provides a generic abstraction layer that allows uniform interrogation of all hosts.

The most frequent use of this function is to obtain a code object for specific code. To do that, pass `NULL` for the `host` parameter and specify all the attributes you have for the guest. You can also use this function to crawl through the guest hosting structure in incremental steps. To do so, pass in a specific host and the attributes for a particular guest.

## See Also

### Related Documentation

func SecCodeCopyHost(SecCode, SecCSFlags, UnsafeMutablePointer&lt;SecCode?>) -> OSStatus

Retrieves the code object for the host of specified guest code.

func SecCodeCopyStaticCode(SecCode, SecCSFlags, UnsafeMutablePointer&lt;SecStaticCode?>) -> OSStatus

Returns a static code object representing the on-disk version of the given running code.

func SecCodeCopySelf(SecCSFlags, UnsafeMutablePointer&lt;SecCode?>) -> OSStatus

Retrieves the code object for the code making the call.

