

- System
- Errno
-  authenticationError 

Type Property

# authenticationError

Authentication error.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var authenticationError: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

The authentication ticket used to mount an NFS file system was invalid.

The corresponding C error is `EAUTH`.

## See Also

### NFS Errors

static var needAuthenticator: Errno

Need authenticator.

static var staleNFSFileHandle: Errno

Stale NFS file handle.

