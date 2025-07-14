

- Game Controller
- GCPhysicalInputElementCollection
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses the collection’s elements using the element’s name.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOS

``` source
subscript(elementName: Name) -> Name.PhysicalInputElement? where Name : GCPhysicalInputElementTypedName { get }
```

Available when `T` conforms to `GCPhysicalInputElement`.

