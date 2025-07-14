

- JavaScriptCore
- JSValue
-  isNull 

Instance Property

# isNull

A Boolean value that indicates whether the instance corresponds to the JavaScript `null` value.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var isNull: Bool { get }
```

## Discussion

The JavaScript `null` value is used only in cases where an actual value is expected but none is applicable. Note that `null` is not the same as `undefined`.

## See Also

### Determining the Type of a JavaScript Value

var isUndefined: Bool

A Boolean value that indicates whether the instance corresponds to the JavaScript `undefined` value.

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

