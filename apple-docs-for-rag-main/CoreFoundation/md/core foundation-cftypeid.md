

- Core Foundation
-  CFTypeID 

Type Alias

# CFTypeID

A type for unique, constant integer values that identify particular Core Foundation opaque types.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CFTypeID = UInt
```

## Discussion

Defines a type identifier in Core Foundation. A type ID is an integer that identifies the opaque type to which a Core Foundation object “belongs.” You use type IDs in various contexts, such as when you are operating on heterogeneous collections. Core Foundation provides programmatic interfaces for obtaining and evaluating type IDs.

Because the value for a type ID can change from release to release, your code should not rely on stored or hard-coded type IDs nor should it hard-code any observed properties of a type ID (such as, for example, it being a small integer).

## See Also

### Data Types

typealias CFHashCode

A type for hash codes returned by the `CFHash` function.

