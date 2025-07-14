

- JavaScriptCore
- JSValue
-  isUndefined 

Instance Property

# isUndefined

A Boolean value that indicates whether the instance corresponds to the JavaScript `undefined` value.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var isUndefined: Bool { get }
```

## Discussion

The JavaScript `undefined` value is used for variables that have not yet been assigned a value, for formal parameters in functions for which no actual parameter has been passed, and as the result of expressions or function calls that do not explicitly return a value. Note that `undefined` is not the same as `null`.

## See Also

### Determining the Type of a JavaScript Value

var isNull: Bool

A Boolean value that indicates whether the instance corresponds to the JavaScript `null` value.

var isBoolean: Bool

A Boolean value that indicates whether the instance is a JavaScript Boolean value.

var isNumber: Bool

A Boolean value that indicates whether the instance is a JavaScript numeric value.

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

