

- CFNetwork
-  CFHTTPAuthenticationCreateFromResponse(\_:\_:) 

Function

# CFHTTPAuthenticationCreateFromResponse(\_:\_:)

Uses an authentication failure response to create a CFHTTPAuthentication object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+

``` source
func CFHTTPAuthenticationCreateFromResponse(
    _ alloc: CFAllocator?,
    _ response: CFHTTPMessage
) -> Unmanaged
```

## Parameters 

`alloc`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`response`  

Response indicating an authentication failure; usually a 401 or a 407 response.

## Return Value

CFHTTPAuthentication object that can be used for adding credentials to future requests. Ownership follows the The Create Rule.

## Discussion

This function uses a response containing authentication failure information to create a reference to a CFHTTPAuthentication object. You can use the object to add credentials to future requests. You can query the object to get the following information:

- whether it can be used and re-used to authenticate with its corresponding server \[CFHTTPAuthenticationIsValid(_:_:)\]

- the authentication method that will be used when it is used to perform an authentication \[CFHTTPAuthenticationCopyMethod(_:)\]

- whether it is associated with a particular CFHTTPMessageRef \[CFHTTPAuthenticationAppliesToRequest(_:_:)

- whether a user name and a password will be required when it is used to perform an authentication \[CFHTTPAuthenticationRequiresUserNameAndPassword(_:)\]

- whether an account domain will be required when it is used to perform an authentication \[CFHTTPAuthenticationRequiresAccountDomain(_:)\]

- whether authentication requests should be sent one at a time to the corresponding server \[CFHTTPAuthenticationRequiresOrderedRequests(_:)\]

- the namespace (if any) that the domain uses to prompt for a name and password \[CFHTTPAuthenticationCopyRealm(_:)\]

- the domain URLs the instance applies to \[CFHTTPAuthenticationCopyDomains(_:)\]

When you have determined what information will be needed to perform the authentication and accumulated that information, call CFHTTPMessageApplyCredentials(_:_:_:_:_:) or CFHTTPMessageApplyCredentialDictionary(_:_:_:_:) to perform the authentication.

## See Also

### HTTP Authentication

class CFHTTPAuthentication

An opaque reference representing HTTP authentication information.

func CFHTTPAuthenticationAppliesToRequest(CFHTTPAuthentication, CFHTTPMessage) -> Bool

Returns a Boolean value that indicates whether a CFHTTPAuthentication object is associated with a CFHTTPMessage object.

func CFHTTPAuthenticationCopyDomains(CFHTTPAuthentication) -> Unmanaged&lt;CFArray>

Returns an array of domain URLs to which a given CFHTTPAuthentication object can be applied.

func CFHTTPAuthenticationCopyMethod(CFHTTPAuthentication) -> Unmanaged&lt;CFString>

Gets the strongest authentication method that will be used when a CFHTTPAuthentication object is applied to a request.

func CFHTTPAuthenticationCopyRealm(CFHTTPAuthentication) -> Unmanaged&lt;CFString>

Gets an authentication information’s namespace.

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

