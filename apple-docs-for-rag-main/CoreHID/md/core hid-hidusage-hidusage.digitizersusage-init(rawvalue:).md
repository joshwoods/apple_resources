

- Core HID
- HIDUsage
- HIDUsage.DigitizersUsage
-  init(rawValue:) 

Initializer

# init(rawValue:)

Creates a new instance with the specified raw value.

macOS 15.0+

``` source
init?(rawValue: UInt16)
```

## Parameters 

`rawValue`  

The raw value to use for the new instance.

## Discussion

If there is no value of the type that corresponds with the specified raw value, this initializer returns `nil`. For example:

```
enum PaperSize: String {
    case A4, A5, Letter, Legal
}

print(PaperSize(rawValue: "Legal"))
// Prints "Optional(PaperSize.Legal)"

print(PaperSize(rawValue: "Tabloid"))
// Prints "nil"
```

