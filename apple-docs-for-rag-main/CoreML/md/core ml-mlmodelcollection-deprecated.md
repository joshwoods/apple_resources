

- Core ML
-  MLModelCollection Deprecated

Class

# MLModelCollection

A set of Core ML models from a model deployment.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedvisionOS 1.0–1.1Deprecated

``` source
class MLModelCollection
```

Deprecated

Use Background Assets or URLSession instead.

## Overview

Use a model collection to access the models from a Core ML Model Deployment. For example, you can use a model collection to replace one or more of your app’s built-in models with a newer version.

To access the newest model collection from a deployment, call the beginAccessingModelCollectionWithIdentifier:completionHandler: type method. Your app can also get a notification when Core ML receives an update to a model collection (see didChangeNotification).

## Topics

### Accessing a Model Collection

class func endAccessing(identifier: String) async throws -> Bool

Terminates access to a model collection.

### Identifying a Model Collection

var identifier: String

The name of the model collection, unique to the development team.

var deploymentID: String

The unique identifier of the model collection’s deployment.

### Retreiving Models from a Collection

var entries: [String : MLModelCollection.Entry]

A dictionary of model entries keyed to the models’ identifiers.

class Entry

A model and its identifier within a model collection.

### Registering for Model Collection Updates

class let didChangeNotification: NSNotification.Name

The notification the framework sends when it receives an update to a model collection.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

