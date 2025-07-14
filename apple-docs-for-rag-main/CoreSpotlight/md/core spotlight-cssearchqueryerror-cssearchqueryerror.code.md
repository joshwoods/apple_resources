

- Core Spotlight
- CSSearchQueryError
-  CSSearchQueryError.Code 

Enumeration

# CSSearchQueryError.Code

Error codes that describe reasons a query might fail.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
enum Code
```

## Topics

### Getting the error codes.

case cancelled

The query stopped because someone canceled it.

case indexUnreachable

The index is unreachable.

case invalidQuery

The query is syntactically invalid or specifies items that your app doesn’t have access to.

case unknown

An unknown error occurred.

### Creating a query error

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

