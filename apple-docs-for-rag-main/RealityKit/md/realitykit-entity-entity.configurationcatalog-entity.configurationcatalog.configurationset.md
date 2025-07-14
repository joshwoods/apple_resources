

- RealityKit
- Entity
- Entity.ConfigurationCatalog
-  Entity.ConfigurationCatalog.ConfigurationSet 

Structure

# Entity.ConfigurationCatalog.ConfigurationSet

A collection of alternatives to choose from.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct ConfigurationSet
```

## Overview

For example, a configuration set might contain configurations named `small`, `medium`, and `big` to represent a choice of sizes.

## Topics

### Creating a configuration set

init(id: String, configurations: [Entity.ConfigurationCatalog.Configuration], defaultConfigurationId: String?) throws

Creates a configuration set from an ID, an array of configurations, and a default configuration ID.

init(id: String, configurations: [String : Entity.ConfigurationCatalog.Configuration], defaultConfigurationId: String?) throws

Creates a configuration set from an ID, a dictionary of configurations, and a default configuration ID.

### Accessing a configuration set’s name

var id: String

A name that identifies the configuration set.

### Accessing configurations in a configuration set

var configurations: [String : Entity.ConfigurationCatalog.Configuration]

The alternative configurations that are available in a set.

var defaultConfiguration: Entity.ConfigurationCatalog.Configuration

The default configuration, if you don’t explicitly set one.

### Type Aliases

typealias ID

A type representing the stable identity of the entity associated with an instance.

## Relationships

### Conforms To

- Identifiable
- Sendable

## See Also

### Defining configuration choices

struct Configuration

A type that represents an alternative that you can choose.

struct ConfigurationCombination

A type that associates an entity with a combination of configurations.

