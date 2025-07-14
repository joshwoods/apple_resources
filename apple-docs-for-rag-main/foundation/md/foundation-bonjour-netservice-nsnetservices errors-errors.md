

- Foundation
- Bonjour
- NetService
-  NSNetServices Errors 

API Collection

# NSNetServices Errors

If an error occurs, the delegate error-handling methods return a dictionary with the following keys.

## Topics

### Constants

class let errorCode: String

This key identifies the error that occurred during the most recent operation.

class let errorDomain: String

This key identifies the originator of the error, which is either the `NSNetService` object or the mach network layer. For most errors, you should not need the value provided by this key.

## See Also

### Constants

enum ErrorCode

These constants identify errors that can occur when accessing net services.

struct Options

These constants specify options for a network service.

