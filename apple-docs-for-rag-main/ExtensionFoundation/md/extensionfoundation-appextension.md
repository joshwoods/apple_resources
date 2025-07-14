

- ExtensionFoundation
-  AppExtension 

Protocol

# AppExtension

Declares a type used by app extensions.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.1+watchOS 9.0+

``` source
protocol AppExtension
```

## Topics

### Creating an App Extension

init()

Creates a new app extension.

**Required**

### Implementing an App Extension

var configuration: Self.Configuration

The configuration object for this app extension.

**Required**

associatedtype Configuration : AppExtensionConfiguration

A type that provides the app extension configuration information.

**Required**

static func main() throws

The main entry point for a non-UI extension.

static func main() throws

The main entry point for a UI extension.

### Default Implementations

AppExtension Implementations

## See Also

### App Extensions

struct AppExtensionIdentity

An object that uniquely identifies an app extension.

protocol AppExtensionConfiguration

An object that holds configuration options for an app extension.

