

- Core Services
- Apple Events
- Constants for Object Specifiers, Positions, and Logical and Comparison Operations
-  kAEMiddle 

Global Variable

# kAEMiddle

Mac Catalyst 13.0+macOS 10.0+

``` source
var kAEMiddle: Int { get }
```

## Discussion

Specifies the middle element in the container. If an object specifier specifies `kAEMiddle` and the number of elements in the container is even, the Apple Event Manager rounds down. For example, in a range of four words the second word is the “middle” word.

