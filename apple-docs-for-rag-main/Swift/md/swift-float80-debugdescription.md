

- Swift
- Float80
-  debugDescription 

Instance Property

# debugDescription

A textual representation of the value, suitable for debugging.

macOS 10.10+

``` source
var debugDescription: String { get }
```

## Discussion

This property has the same value as the `description` property, except that NaN values are printed in an extended format.

