

- ExtensionFoundation
- AppExtension
-  main() 

Type Method

# main()

The main entry point for a non-UI extension.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.1+watchOS 9.0+

``` source
@MainActor @preconcurrency
static func main() throws
```

## See Also

### Implementing an App Extension

var configuration: Self.Configuration

The configuration object for this app extension.

**Required**

associatedtype Configuration : AppExtensionConfiguration

A type that provides the app extension configuration information.

**Required**

static func main() throws

The main entry point for a UI extension.

