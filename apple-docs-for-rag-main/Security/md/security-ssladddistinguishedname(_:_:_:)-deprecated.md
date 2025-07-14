

- Security
-  SSLAddDistinguishedName(\_:\_:\_:) Deprecated

Function

# SSLAddDistinguishedName(\_:\_:\_:)

Adds a DER-encoded distinguished name to a list of acceptable names to be specified in requests for client certificates.

iOS 5.0–13.0DeprecatediPadOS 5.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.4–10.15Deprecated

``` source
func SSLAddDistinguishedName(
    _ context: SSLContext,
    _ derDN: UnsafeRawPointer?,
    _ derDNLen: Int
) -> OSStatus
```

Deprecated

No longer supported. Use Network.framework.

## Parameters 

`context`  

An SSL session context reference.

`derDN`  

A pointer to a buffer containing a DER-encoded distinguished name.

`derDNLen`  

A value of type `size_t` representing the size of the buffer pointed to by the parameter `derDN`.

## Return Value

A result code. See Secure Transport Result Codes.

