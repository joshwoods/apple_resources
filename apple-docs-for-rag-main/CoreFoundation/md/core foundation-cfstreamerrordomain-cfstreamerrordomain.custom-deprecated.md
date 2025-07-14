

- Core Foundation
- CFStreamErrorDomain
-  CFStreamErrorDomain.custom Deprecated

Case

# CFStreamErrorDomain.custom

The error code is a custom error code.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
case custom
```

Deprecated

These constants are returned by CFReadStreamGetError(_:) and CFWriteStreamGetError(_:); use CFReadStreamCopyError(_:) and CFWriteStreamCopyError(_:) instead.

## See Also

### Constants

case POSIX

The error code is an error code defined in `errno.h`.

case macOSStatus

The error is an OSStatus value defined in `MacErrors.h`.

