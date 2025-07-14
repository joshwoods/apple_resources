

- Core Services
- Launch Services
-  LSHandlerOptions 

Structure

# LSHandlerOptions

The specification that controls the selection of handlers.

Mac Catalyst 13.0+macOS 10.4+

``` source
struct LSHandlerOptions
```

## Topics

### Creating Content Handler Options

init(rawValue: OptionBits)

### Constants

static var ignoreCreator: LSHandlerOptions

When set, causes Launch Services to ignorethe content item’s creator when selecting a role handler for thespecified content type.

Deprecated

## Relationships

### Conforms To

- OptionSet
- Sendable

