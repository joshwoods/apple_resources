

- Core Services
- Apple Events
- Key Form and Descriptor Type Object Specifier Constants
-  formTest 

Global Variable

# formTest

Mac Catalyst 13.0+macOS 10.0+

``` source
var formTest: Int { get }
```

## Discussion

Specifies a test. The key data is specified by either a comparison descriptor or a logical descriptor.

The Apple Event Manager internally translates object specifiers of key form `formTest` into object specifiers of key form `formWhose` to optimize resolution of object specifiers. This involves collapsing the key form and key data from two object specifiers in a container hierarchy into one object specifier with the key form `formWhose`.

See also AEDisposeToken(_:), Constants for Object Specifiers, Positions, and Logical and Comparison Operations, CreateCompDescriptor(_:_:_:_:_:), and CreateLogicalDescriptor(_:_:_:_:).

