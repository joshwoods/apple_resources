

- JavaScriptCore
- JSValue
-  isNumber 

Instance Property

# isNumber

A Boolean value that indicates whether the instance is a JavaScript numeric value.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var isNumber: Bool { get }
```

## Discussion

In JavaScript, there is no differentiation between types of numbers. Semantically, all numbers behave as double-precision floating-point types, except in special cases like bit operations.

## See Also

### Determining the Type of a JavaScript Value

var isUndefined: Bool

A Boolean value that indicates whether the instance corresponds to the JavaScript `undefined` value.

var isNull: Bool

A Boolean value that indicates whether the instance corresponds to the JavaScript `null` value.

var isBoolean: Bool

A Boolean value that indicates whether the instance is a JavaScript Boolean value.

var isString: Bool

A Boolean value that indicates whether the instance is a JavaScript `String` object.

var isObject: Bool

A Boolean value that indicates whether the instance is a JavaScript object.

var isArray: Bool

A Boolean value that indicates whether the instance is a JavaScript array value.

var isDate: Bool

A Boolean value that indicates whether the instance is a JavaScript `Date` object.

var isSymbol: Bool

A Boolean value that indicates whether the instance is a symbol.

