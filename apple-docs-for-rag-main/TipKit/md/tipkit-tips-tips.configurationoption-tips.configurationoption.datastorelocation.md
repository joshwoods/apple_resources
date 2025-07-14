

- TipKit
- Tips
- Tips.ConfigurationOption
-  Tips.ConfigurationOption.DatastoreLocation 

Structure

# Tips.ConfigurationOption.DatastoreLocation

A type for specifying a custom location for your tips datastore.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct DatastoreLocation
```

## Overview

For more information on datastore location, see datastoreLocation(_:).

## Topics

### Type Properties

static var applicationDefault: Tips.ConfigurationOption.DatastoreLocation

The default location for persisting tips, which is generally your application’s support directory.

### Type Methods

static func groupContainer(identifier: String) throws -> Tips.ConfigurationOption.DatastoreLocation

DatastoreLocation for persisting tips in a group container.

static func url(URL) -> Tips.ConfigurationOption.DatastoreLocation

DatastoreLocation for persisting tips at a custom URL.

## Relationships

### Conforms To

- Equatable
- Sendable

