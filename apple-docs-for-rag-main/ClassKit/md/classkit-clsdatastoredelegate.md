

- ClassKit
-  CLSDataStoreDelegate 

Protocol

# CLSDataStoreDelegate

An interface the data store uses to request new contexts.

iOS 11.3+iPadOS 11.3+Mac Catalyst 11.3+macOS 11.0+visionOS 1.0+

``` source
protocol CLSDataStoreDelegate : NSObjectProtocol
```

## Mentioned in 

Building missing contexts

## Overview

When you request a context from the data store, for example using a call to the descendant(matchingIdentifierPath:completion:) method, the data store first tries to locate an existing context matching the search criterion (an identifier path in this case) in its database. Depending on certain conditions, the context might already exist in the database from the last time you requested it. If it does, the data store returns the stored context. But if it doesn’t exist, the data store asks its delegate to build a new context.

Adopt the data store delegate protocol to provide contexts on demand.

You can alternatively build contexts directly without relying on the delegate callback. However, it’s generally most efficient to use the delegate protocol, building contexts only when they’re missing from the data store.

## Topics

### Creating Contexts

func createContext(forIdentifier: String, parentContext: CLSContext, parentIdentifierPath: [String]) -> CLSContext?

Asks the delegate for a new context with the given identifier for the given parent context.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Managing the delegate

Building missing contexts

Create and initialize missing contexts.

var delegate: (any CLSDataStoreDelegate)?

The data store delegate instance.

