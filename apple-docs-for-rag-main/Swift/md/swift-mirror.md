

- Swift
-  Mirror 

Structure

# Mirror

A representation of the substructure and display style of an instance of any type.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct Mirror
```

## Overview

A mirror describes the parts that make up a particular instance, such as the instance’s stored properties, collection or tuple elements, or its active enumeration case. Mirrors also provide a “display style” property that suggests how this mirror might be rendered.

Playgrounds and the debugger use the `Mirror` type to display representations of values of any type. For example, when you pass an instance to the `dump(_:_:_:_:)` function, a mirror is used to render that instance’s runtime contents.

```
struct Point {
    let x: Int, y: Int
}

let p = Point(x: 21, y: 30)
print(String(reflecting: p))
// Prints "▿ Point
//           - x: 21
//           - y: 30"
```

To customize the mirror representation of a custom type, add conformance to the `CustomReflectable` protocol.

## Topics

### Querying Descendants

func descendant(any MirrorPath, any MirrorPath...) -> Any?

Returns a specific descendant of the reflected subject, or `nil` if no such descendant exists.

protocol MirrorPath

A protocol for legitimate arguments to `Mirror`’s `descendant` method.

### Initializers

init&lt;Subject>(Subject, children: KeyValuePairs&lt;String, Any>, displayStyle: Mirror.DisplayStyle?, ancestorRepresentation: Mirror.AncestorRepresentation)

Creates a mirror representing the given subject using a dictionary literal for the structure.

init&lt;Subject, C>(Subject, children: C, displayStyle: Mirror.DisplayStyle?, ancestorRepresentation: Mirror.AncestorRepresentation)

Creates a mirror representing the given subject with a specified structure.

init&lt;Subject, C>(Subject, unlabeledChildren: C, displayStyle: Mirror.DisplayStyle?, ancestorRepresentation: Mirror.AncestorRepresentation)

Creates a mirror representing the given subject with unlabeled children.

init(reflecting: Any)

Creates a mirror that reflects on the given instance.

### Instance Properties

let children: Mirror.Children

A collection of `Child` elements describing the structure of the reflected subject.

let displayStyle: Mirror.DisplayStyle?

A suggested display style for the reflected subject.

let subjectType: any Any.Type

The static type of the subject being reflected.

var superclassMirror: Mirror?

A mirror of the subject’s superclass, if one exists.

### Type Aliases

typealias Child

An element of the reflected instance’s structure.

typealias Children

The type used to represent substructure.

### Enumerations

enum AncestorRepresentation

The representation to use for ancestor classes.

enum DisplayStyle

A suggestion of how a mirror’s subject is to be interpreted.

### Default Implementations

CustomReflectable Implementations

CustomStringConvertible Implementations

## Relationships

### Conforms To

- Copyable
- CustomReflectable
- CustomStringConvertible

## See Also

### Querying Runtime Values

struct ObjectIdentifier

A unique identifier for a class instance or metatype.

func type&lt;T, Metatype>(of: T) -> Metatype

Returns the dynamic type of a value.

func == ((any Any.Type)?, (any Any.Type)?) -> Bool

Returns a Boolean value indicating whether two types are identical.

func != ((any Any.Type)?, (any Any.Type)?) -> Bool

Returns a Boolean value indicating whether two types are not identical.

