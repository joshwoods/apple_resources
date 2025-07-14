

- Core Spotlight
- CSSearchQueryError
-  cancelled 

Type Property

# cancelled

The query stopped because someone canceled it.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
static var cancelled: CSSearchQueryError.Code { get }
```

## Discussion

The system reports this error if your code called the cancel() method.

## See Also

### Getting the error codes

static var indexUnreachable: CSSearchQueryError.Code

The index is unreachable.

static var invalidQuery: CSSearchQueryError.Code

The query is syntactically invalid or specifies items that your app doesn’t have access to.

static var unknown: CSSearchQueryError.Code

An unknown error occurred.

