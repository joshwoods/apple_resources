

- ShazamKit
- SHSession
-  result(from:) 

Instance Method

# result(from:)

Performs an asynchronous match with a signature you specify.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func result(from signature: SHSignature) async -> SHSession.Result
```

## Parameters 

`signature`  

The signature to match.

## Return Value

A SHSession.Result enum that indicates the result.

## See Also

### Returning queries

enum Result

Identifies the result from an asynchronous sequence result.

