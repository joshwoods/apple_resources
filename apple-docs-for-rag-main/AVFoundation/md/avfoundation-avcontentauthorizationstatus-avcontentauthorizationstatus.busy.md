

- AVFoundation
- AVContentAuthorizationStatus
-  AVContentAuthorizationStatus.busy 

Case

# AVContentAuthorizationStatus.busy

The last call to request content authorization couldn’t be completed because another asset is currently attempting authorization.

macOS

``` source
case busy
```

## See Also

### Content Authorization Statuses

case unknown

The content authorization content request hasn’t completed.

case completed

The last completed call to request content authorization completed.

case cancelled

The last call to request content authorization was cancelled by the user.

case timedOut

The last call to request content authorization was cancelled because the timeout interval was reached.

case notAvailable

The last call to request content authorization couldn’t be completed because there was no known mechanism by which to attempt authorization.

case notPossible

The last call to request content authorization couldn’t be completed in a non-recoverable way.

