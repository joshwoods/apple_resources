

- File Provider
-  NSFileProviderDomainVersion 

Class

# NSFileProviderDomainVersion

An opaque object that identifies a specific version of a domain.

iOS 16.0+iPadOS 16.0+macOS 11.3+visionOS 1.0+

``` source
class NSFileProviderDomainVersion
```

## Overview

The file provider extension is responsible for assigning and updating the domain version. To specify the domain version, adopt the NSFileProviderDomainState protocol. The system then calls your extension’s domainVersion method to read the current version.

The system reads the domain version after you call:

- The createItem(basedOn:fields:contents:options:request:completionHandler:) completion handler

- The modifyItem(_:baseVersion:changedFields:contents:options:request:completionHandler:) completion handler

- The deleteItem(identifier:baseVersion:options:request:completionHandler:) completion handler

- The item(for:request:completionHandler:) completion handler

- The finishEnumerating(upTo:) or finishEnumeratingWithError(_:) method when enumerating the materialized set.

The system always reads the domain version on the same dispatch queue as the completion handler.

Your extension defines when the domain version changes. When you update the version, call the signalEnumerator(for:completionHandler:) and passing the workingSet constant as the `containerItemIdentifier` property. This notifies the system of the update. The system ignores any lower versions.

When the system discovers a change on disk, it associates that change with the current domain version. It then includes the version in the NSFileProviderRequest object passed to the file provider extension.

Only file provider extensions based on the NSFileProviderReplicatedExtension use instances of this class. Each version object is immutable. You can use them as keys in a dictionary.

## Topics

### Creating Versions

func next() -> NSFileProviderDomainVersion

Creates a new version that supersedes the current version.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- Comparable
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Domains

protocol NSFileProviderDomainState

An object that contains global state data about the domain.

