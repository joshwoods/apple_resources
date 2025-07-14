

- CFNetwork
-  CFHTTPAuthenticationAppliesToRequest(\_:\_:) 

Function

# CFHTTPAuthenticationAppliesToRequest(\_:\_:)

Returns a Boolean value that indicates whether a CFHTTPAuthentication object is associated with a CFHTTPMessage object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+

``` source
func CFHTTPAuthenticationAppliesToRequest(
    _ auth: CFHTTPAuthentication,
    _ request: CFHTTPMessage
) -> Bool
```

## Parameters 

`auth`  

The CFHTTPAuthentication object to examine.

`request`  

Request that `auth` is to be tested against.

## Return Value

`TRUE` if `auth` is associated with `request`, otherwise `FALSE`.

## Discussion

If this function returns `TRUE`, you can use `auth` to provide authentication information when using `request`.

## See Also

### HTTP Authentication

class CFHTTPAuthentication

An opaque reference representing HTTP authentication information.

func CFHTTPAuthenticationCopyDomains(CFHTTPAuthentication) -> Unmanaged&lt;CFArray>

Returns an array of domain URLs to which a given CFHTTPAuthentication object can be applied.

func CFHTTPAuthenticationCopyMethod(CFHTTPAuthentication) -> Unmanaged&lt;CFString>

Gets the strongest authentication method that will be used when a CFHTTPAuthentication object is applied to a request.

func CFHTTPAuthenticationCopyRealm(CFHTTPAuthentication) -> Unmanaged&lt;CFString>

Gets an authentication information’s namespace.

func CFHTTPAuthenticationCreateFromResponse(CFAllocator?, CFHTTPMessage) -> Unmanaged&lt;CFHTTPAuthentication>

Uses an authentication failure response to create a CFHTTPAuthentication object.

func CFHTTPAuthenticationGetTypeID() -> CFTypeID

Gets the Core Foundation type identifier for the CFHTTPAuthentication opaque type.

func CFHTTPAuthenticationIsValid(CFHTTPAuthentication, UnsafeMutablePointer&lt;CFStreamError>?) -> Bool

Returns a Boolean value that indicates whether a CFHTTPAuthentication object is valid.

func CFHTTPAuthenticationRequiresAccountDomain(CFHTTPAuthentication) -> Bool

Returns a Boolean value that indicates whether a CFHTTPAuthentication object uses an authentication method that requires an account domain.

func CFHTTPAuthenticationRequiresOrderedRequests(CFHTTPAuthentication) -> Bool

Returns a Boolean value that indicates whether authentication requests should be made one at a time.

func CFHTTPAuthenticationRequiresUserNameAndPassword(CFHTTPAuthentication) -> Bool

Returns a Boolean value that indicates whether a CFHTTPAuthentication object uses an authentication method that requires a username and a password.

let kCFHTTPAuthenticationAccountDomain: CFString

Account domain to use for authentication.

let kCFHTTPAuthenticationPassword: CFString

Password to use for authentication.

let kCFHTTPAuthenticationSchemeBasic: CFString

Request the HTTP basic authentication scheme.

let kCFHTTPAuthenticationSchemeDigest: CFString

Request the HTTP digest authentication scheme.

let kCFHTTPAuthenticationSchemeKerberos: CFString

Request the HTTP Kerberos authentication scheme.

