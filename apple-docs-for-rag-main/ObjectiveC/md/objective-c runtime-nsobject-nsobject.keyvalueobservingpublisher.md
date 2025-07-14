

- Objective-C Runtime
- NSObject
-  NSObject.KeyValueObservingPublisher 

Structure

# NSObject.KeyValueObservingPublisher

A Combine publisher that produces a new element whenever the observed value changes.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
struct KeyValueObservingPublisher where Subject : NSObject
```

## Overview

Use this publisher to integrate a property that’s compliant with key-value observing into a Combine publishing chain. You can create a publisher of this type with the NSObject instance method `publisher(for:options:)`, passing in the key path and a set of NSKeyValueObservingOptions.

## Topics

### Creating a KVO Publisher

init(object: Subject, keyPath: KeyPath&lt;Subject, Value>, options: NSKeyValueObservingOptions)

Creates a key-value observing publisher for the given combination of object and key path, using publishing behavior options you provide.

### Inspecting KVO Publisher Properties

let object: Subject

The object that contains the property to publish.

let keyPath: KeyPath&lt;Subject, Value>

The key path, relative to the object receiving this message, of the property to publish.

let options: NSKeyValueObservingOptions

Options that determine which elements the publisher produces.

### Instance Methods

func didChange() -> Publishers.Map&lt;NSObject.KeyValueObservingPublisher&lt;Subject, Value>, Void>

Returns a publisher that emits values when a KVO-compliant property changes.

## Relationships

### Conforms To

- Copyable
- Equatable
- Publisher

