

- Core Spotlight
- CSSearchQueryError
- CSSearchQueryError.Code
-  CSSearchQueryError.Code.cancelled 

Case

# CSSearchQueryError.Code.cancelled

The query stopped because someone canceled it.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
case cancelled
```

## Discussion

The system reports this error if your code called the cancel() method.

## See Also

### Getting the error codes.

case indexUnreachable

The index is unreachable.

case invalidQuery

The query is syntactically invalid or specifies items that your app doesn’t have access to.

case unknown

An unknown error occurred.

