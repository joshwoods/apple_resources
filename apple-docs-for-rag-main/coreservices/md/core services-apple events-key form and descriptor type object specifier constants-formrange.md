

- Core Services
- Apple Events
- Key Form and Descriptor Type Object Specifier Constants
-  formRange 

Global Variable

# formRange

Mac Catalyst 13.0+macOS 10.0+

``` source
var formRange: Int { get }
```

## Discussion

Specifies a group of elements between two other elements. The key data is specified by a range descriptor, which is a coerced Apple event record of type `typeRangeDescriptor` that identifies two Apple event objects marking the beginning and end of a range of elements.

The data for a range descriptor consists of two keyword-specified descriptors with the keywords `keyAERangeStart` and `keyAERangeStop`.

