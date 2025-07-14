

- RealityKit
- Entity
- Entity.ConfigurationCatalog
-  Entity.ConfigurationCatalog.Configuration 

Structure

# Entity.ConfigurationCatalog.Configuration

A type that represents an alternative that you can choose.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct Configuration
```

## Topics

### Creating a configuration

init(id: String)

Creates a configuration with an identifier.

### Accessing a configuration’s name

var id: String

A name that identifies the configuration.

### Type Aliases

typealias ID

A type representing the stable identity of the entity associated with an instance.

## Relationships

### Conforms To

- Identifiable
- Sendable

## See Also

### Defining configuration choices

struct ConfigurationSet

A collection of alternatives to choose from.

struct ConfigurationCombination

A type that associates an entity with a combination of configurations.

