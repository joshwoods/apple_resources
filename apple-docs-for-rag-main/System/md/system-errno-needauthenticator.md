

- System
- Errno
-  needAuthenticator 

Type Property

# needAuthenticator

Need authenticator.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var needAuthenticator: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

Before mounting the given NFS file system, you must obtain an authentication ticket.

The corresponding C error is `ENEEDAUTH`.

## See Also

### NFS Errors

static var authenticationError: Errno

Authentication error.

static var staleNFSFileHandle: Errno

Stale NFS file handle.

