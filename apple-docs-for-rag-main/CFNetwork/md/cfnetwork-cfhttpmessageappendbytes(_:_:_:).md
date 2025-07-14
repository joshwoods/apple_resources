

- CFNetwork
-  CFHTTPMessageAppendBytes(\_:\_:\_:) 

Function

# CFHTTPMessageAppendBytes(\_:\_:\_:)

Appends data to a `CFHTTPMessage` object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.1+tvOS 9.0+visionOS 1.0+

``` source
func CFHTTPMessageAppendBytes(
    _ message: CFHTTPMessage,
    _ newBytes: UnsafePointer,
    _ numBytes: CFIndex
) -> Bool
```

## Parameters 

`message`  

The message to modify.

`newBytes`  

A reference to the data to append.

`numBytes`  

The length of the data pointed to by `newBytes`.

## Return Value

`TRUE` if the data was successfully appended, otherwise `FALSE`.

## Discussion

This function appends the data specified by `newBytes` to the specified message object which was created by calling CFHTTPMessageCreateEmpty(_:_:). The data is an incoming serialized HTTP request or response received from a client or a server. While appending the data, this function deserializes it, removes any HTTP-based formatting that the message may contain, and stores the message in the message object. You can then call CFHTTPMessageCopyVersion(_:), CFHTTPMessageCopyBody(_:), CFHTTPMessageCopyHeaderFieldValue(_:_:), and CFHTTPMessageCopyAllHeaderFields(_:) to get the message’s HTTP version, the message’s body, a specific header field, and all of the message’s headers, respectively.

If the message is a request, you can also call CFHTTPMessageCopyRequestURL(_:) and CFHTTPMessageCopyRequestMethod(_:) to get the message’s request URL and request method, respectively.

If the message is a response, you can also call CFHTTPMessageGetResponseStatusCode(_:) and CFHTTPMessageCopyResponseStatusLine(_:) to get the message’s status code and status line, respectively.

## See Also

### HTTP Messages

class CFHTTPMessage

An opaque reference representing an HTTP message.

func CFHTTPMessageAddAuthentication(CFHTTPMessage, CFHTTPMessage?, CFString, CFString, CFString?, Bool) -> Bool

Adds authentication information to a request.

func CFHTTPMessageApplyCredentialDictionary(CFHTTPMessage, CFHTTPAuthentication, CFDictionary, UnsafeMutablePointer&lt;CFStreamError>?) -> Bool

Use a dictionary containing authentication credentials to perform the authentication method specified by a `CFHTTPAuthentication` object.

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

