

- CFNetwork
-  CFHTTPMessageApplyCredentialDictionary(\_:\_:\_:\_:) 

Function

# CFHTTPMessageApplyCredentialDictionary(\_:\_:\_:\_:)

Use a dictionary containing authentication credentials to perform the authentication method specified by a `CFHTTPAuthentication` object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
func CFHTTPMessageApplyCredentialDictionary(
    _ request: CFHTTPMessage,
    _ auth: CFHTTPAuthentication,
    _ dict: CFDictionary,
    _ error: UnsafeMutablePointer?
) -> Bool
```

## Parameters 

`request`  

The request for which the authentication method is to be performed.

`auth`  

A `CFHTTPAuthentication` object specifying the authentication method to perform.

`dict`  

A dictionary containing authentication credentials to be applied to the request. For information on the keys in this dictionary, see CFHTTPAuthentication.

`error`  

If an error occurs, upon return contains a CFStreamError object that describes the error and the error’s domain. Pass `NULL` if you don’t want to receive error information.

## Return Value

`TRUE` if the authentication was successful, otherwise, `FALSE`.

## Discussion

This function performs the authentication method specified by `auth` on behalf of the request specified by `request` using the credentials contained in the dictionary specified by `dict`. The dictionary must contain values for the `kCFHTTPAuthenticationUsername` and `kCFHTTPAuthenticationPassword` keys. If CFHTTPAuthenticationRequiresAccountDomain(_:) returns `TRUE` for `auth`, the dictionary must also contain a value for the `kCFHTTPAuthenticationAccountDomain` key.

### Special Considerations

This function is thread safe as long as another thread does not alter the same `CFHTTPAuthentication` object at the same time.

## See Also

### HTTP Messages

class CFHTTPMessage

An opaque reference representing an HTTP message.

func CFHTTPMessageAddAuthentication(CFHTTPMessage, CFHTTPMessage?, CFString, CFString, CFString?, Bool) -> Bool

Adds authentication information to a request.

func CFHTTPMessageAppendBytes(CFHTTPMessage, UnsafePointer&lt;UInt8>, CFIndex) -> Bool

Appends data to a `CFHTTPMessage` object.

func CFHTTPMessageApplyCredentials(CFHTTPMessage, CFHTTPAuthentication, CFString?, CFString?, UnsafeMutablePointer&lt;CFStreamError>?) -> Bool

Performs the authentication method specified by a `CFHTTPAuthentication` object.

func CFHTTPMessageCopyAllHeaderFields(CFHTTPMessage) -> Unmanaged&lt;CFDictionary>?

Gets all header fields from a `CFHTTPMessage` object.

func CFHTTPMessageCopyBody(CFHTTPMessage) -> Unmanaged&lt;CFData>?

Gets the body from a `CFHTTPMessage` object.

func CFHTTPMessageCopyHeaderFieldValue(CFHTTPMessage, CFString) -> Unmanaged&lt;CFString>?

Gets the value of a header field from a `CFHTTPMessage` object.

func CFHTTPMessageCopyRequestMethod(CFHTTPMessage) -> Unmanaged&lt;CFString>?

Gets the request method from a `CFHTTPMessage` object.

func CFHTTPMessageCopyRequestURL(CFHTTPMessage) -> Unmanaged&lt;CFURL>?

Gets the URL from a `CFHTTPMessage` object.

func CFHTTPMessageCopyResponseStatusLine(CFHTTPMessage) -> Unmanaged&lt;CFString>?

Gets the status line from a `CFHTTPMessage` object.

func CFHTTPMessageCopySerializedMessage(CFHTTPMessage) -> Unmanaged&lt;CFData>?

Serializes a CFHTTPMessage object.

func CFHTTPMessageCopyVersion(CFHTTPMessage) -> Unmanaged&lt;CFString>

Gets the HTTP version from a `CFHTTPMessage` object.

func CFHTTPMessageCreateCopy(CFAllocator?, CFHTTPMessage) -> Unmanaged&lt;CFHTTPMessage>

Gets a copy of a CFHTTPMessage object.

func CFHTTPMessageCreateEmpty(CFAllocator?, Bool) -> Unmanaged&lt;CFHTTPMessage>

Creates and returns a new, empty `CFHTTPMessage` object.

func CFHTTPMessageCreateRequest(CFAllocator?, CFString, CFURL, CFString) -> Unmanaged&lt;CFHTTPMessage>

Creates and returns a `CFHTTPMessage` object for an HTTP request.

