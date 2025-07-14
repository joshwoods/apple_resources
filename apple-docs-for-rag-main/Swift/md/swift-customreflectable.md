

- Swift
-  CustomReflectable 

Protocol

# CustomReflectable

A type that explicitly supplies its own mirror.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol CustomReflectable
```

## Overview

You can create a mirror for any type using the `Mirror(reflecting:)` initializer, but if you are not satisfied with the mirror supplied for your type by default, you can make it conform to `CustomReflectable` and return a custom `Mirror` instance.

## Topics

### Instance Properties

var customMirror: Mirror

The custom mirror for this instance.

**Required**

## Relationships

### Inherited By

- CustomLeafReflectable

### Conforming Types

- AnyHashable
- Array

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- ArraySlice

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- AutoreleasingUnsafeMutablePointer
- Bool
- Character
- ClosedRange

  Conforms when `Bound` conforms to `Comparable`.

- CollectionOfOne

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- ContiguousArray

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- Dictionary

  Conforms when `Key` conforms to `Hashable`, `Value` conforms to `Copyable`, and `Value` conforms to `Escapable`.

- Dictionary.Iterator

  Conforms when `Key` conforms to `Hashable`, `Value` conforms to `Copyable`, and `Value` conforms to `Escapable`.

- Double
- Float
- Float80
- Int
- Int128
- Int16
- Int32
- Int64
- Int8
- Mirror
- Optional

  Conforms when `Wrapped` conforms to `Copyable` and `Escapable`.

- Range

  Conforms when `Bound` conforms to `Comparable`.

- Set

  Conforms when `Element` conforms to `Hashable`.

- Set.Iterator

  Conforms when `Element` conforms to `Hashable`.

- StaticBigInt
- StaticString
- StrideThrough

  Conforms when `Element` conforms to `Strideable`.

- StrideTo

  Conforms when `Element` conforms to `Strideable`.

- String
- String.UTF16View
- String.UTF8View
- String.UnicodeScalarView
- Substring
- UInt
- UInt128
- UInt16
- UInt32
- UInt64
- UInt8
- Unicode.Scalar
- UnsafeMutablePointer

  Conforms when `Pointee` conforms to `Escapable`.

- UnsafeMutableRawPointer
- UnsafePointer

  Conforms when `Pointee` conforms to `Escapable`.

- UnsafeRawPointer

## See Also

### Customizing Your Type’s Reflection

protocol CustomLeafReflectable

A type that explicitly supplies its own mirror, but whose descendant classes are not represented in the mirror unless they also override `customMirror`.

protocol CustomPlaygroundDisplayConvertible

A type that supplies a custom description for playground logging.

typealias PlaygroundQuickLook

The sum of types that can be used as a Quick Look representation.

macro DebugDescription()

Converts description definitions to a debugger Type Summary.

