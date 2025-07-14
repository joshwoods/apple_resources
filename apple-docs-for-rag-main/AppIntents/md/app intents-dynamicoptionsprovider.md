

- App Intents
-  DynamicOptionsProvider 

Protocol

# DynamicOptionsProvider

An interface for providing a dynamic list of options for a parameter of your app intent.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol DynamicOptionsProvider : _SupportsAppDependencies
```

## Mentioned in 

Adding parameters to an app intent

## Overview

Implement this protocol in a type that provides a set of possible values for an intent parameter. When configuring the parameter, specify your custom type as the options provider for that parameter. The type of result you return determines how the system displays the information.

- Return an array of DisplayRepresentable types to display a list of values.

- Return an array of IntentItem types to divide values into sections or configure other presentation options.

The following example shows the configuration of a custom parameter that contains the author name of a book. The options provider offers two possible suggestions for the author name. For brevity, it omits the rest of the implementation.

```
struct CreateBook: AppIntent {
    @Parameter(title: "Author Name",
               optionsProvider: AuthorNamesOptionsProvider())
    var authorName: String

    // Other properties and the perform() implementation.

    private struct AuthorNamesOptionsProvider: DynamicOptionsProvider {
        func results() async throws -> [String] {
            ["Juan Chavez", "Anne Johnson"]
        }
    }
}
```

## Topics

### Returning the parameter options

func results() async throws -> Self.Result

**Required** Default implementation provided.

func defaultResult() async -> Self.DefaultValue?

The default value for parameters using this provider when no value is provided by the user.

**Required** Default implementation provided.

associatedtype Result : ResultsCollection

**Required**

### Associated Types

associatedtype DefaultValue : _IntentValue = Self.Result.Result

**Required**

### Type Aliases

typealias Item

typealias ItemCollection

typealias ItemSection

typealias ParameterDependency

## Relationships

### Inherited By

- EntityPropertyQuery
- EntityQuery
- EntityStringQuery
- EnumerableEntityQuery
- UniqueAppEntityQuery

### Conforming Types

- UniqueAppEntityProvider

## See Also

### Parameter choices

protocol AppEnum

An interface to express that a custom type has a predefined, static set of valid values to display.

