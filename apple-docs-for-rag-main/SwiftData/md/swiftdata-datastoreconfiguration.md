

- SwiftData
-  DataStoreConfiguration 

Protocol

# DataStoreConfiguration

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+Swift 5.9+

``` source
protocol DataStoreConfiguration : Hashable
```

## Topics

### Associated Types

associatedtype Store : DataStore

**Required**

### Instance Properties

var name: String

**Required**

var schema: Schema?

**Required**

### Instance Methods

func validate() throws

**Required** Default implementation provided.

## Relationships

### Inherits From

- Equatable
- Hashable

### Conforming Types

- ModelConfiguration

## See Also

### Accessing store information

var configuration: Self.Configuration

**Required**

associatedtype Configuration : DataStoreConfiguration

**Required**

var identifier: String

**Required**

var schema: Schema

**Required**

