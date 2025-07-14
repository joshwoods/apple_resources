

- System
- Errno
-  staleNFSFileHandle 

Type Property

# staleNFSFileHandle

Stale NFS file handle.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var staleNFSFileHandle: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

You attempted access an open file on an NFS filesystem, which is now unavailable as referenced by the given file descriptor. This may indicate that the file was deleted on the NFS server or that some other catastrophic event occurred.

The corresponding C error is `ESTALE`.

## See Also

### NFS Errors

static var authenticationError: Errno

Authentication error.

static var needAuthenticator: Errno

Need authenticator.

