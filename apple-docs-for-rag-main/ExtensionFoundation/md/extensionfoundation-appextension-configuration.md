

- ExtensionFoundation
- AppExtension
-  configuration 

Instance Property

# configuration

The configuration object for this app extension.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.1+watchOS 9.0+

``` source
@MainActor @preconcurrency
var configuration: Self.Configuration { get }
```

**Required**

## See Also

### Implementing an App Extension

associatedtype Configuration : AppExtensionConfiguration

A type that provides the app extension configuration information.

**Required**

static func main() throws

The main entry point for a non-UI extension.

static func main() throws

The main entry point for a UI extension.

