

- Game Controller
- GCPhysicalInputElementCollection
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses a contiguous subrange of a collection of axis elements.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOS

``` source
subscript(elementName: GCAxisElementName) -> T? { get }
```

Available when `T` is `any GCAxisElement`.

## See Also

### Accessing elements by name

subscript(GCDirectionPadElementName) -> T?

Accesses a contiguous subrange of a collection of direction pad elements.

subscript(GCButtonElementName) -> T?

Accesses a contiguous subrange of a collection of button elements.

subscript(GCSwitchElementName) -> T?

Accesses a contiguous subrange of a collection of switch elements.

subscript(GCPhysicalInputElementName) -> T?

