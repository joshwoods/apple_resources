

- Core Spotlight
- CSSearchQueryContext
-  CSSearchQueryContext.SourceOptions 

Structure

# CSSearchQueryContext.SourceOptions

The query source options to allow or deny Mail messages in the search.

iOS 9.0+iPadOS 9.0+Mac Catalyst 16.1+macOS 13.0+visionOS 1.0+

``` source
struct SourceOptions
```

## Topics

### Search options

static var allowMail: CSSearchQueryContext.SourceOptions

The query allows Mail messages in the search.

### Initializers

init(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Configuring search behavior

var fetchAttributes: [String]

The attributes the system fetches for the searchable items.

var keyboardLanguage: String?

The language used for the query.

var sourceOptions: CSSearchQueryContext.SourceOptions

The query source options to allow or deny Mail messages in the search.

