

- JavaScriptCore
- JSValue
-  toString() 

Instance Method

# toString()

Converts the JavaScript value to a native string.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
func toString() -> String!
```

## Return Value

The string representation of the value.

## Discussion

This method uses JavaScript type coercion rules to convert the value to a JavaScript string, then creates a native string from the result. Thus, this method can return a string even when the isString property is false; for example, an empty object becomes the string `"[object Object]"`.

## See Also

### Reading and Converting JavaScript Values

func toObject() -> Any!

Converts the JavaScript value to a native object.

func toObjectOf(AnyClass!) -> Any!

Converts the JavaScript value to a native object of the specified class.

func toBool() -> Bool

Converts the JavaScript value to a native Boolean value.

func toDouble() -> Double

Converts the JavaScript value to a native floating-point value.

func toInt32() -> Int32

Converts the JavaScript value to a native signed integer value.

func toUInt32() -> UInt32

Converts the JavaScript value to a native unsigned integer value.

func toNumber() -> NSNumber!

Converts the JavaScript value to a NSNumber object.

func toDate() -> Date!

Converts the JavaScript value to a date object.

func toArray() -> [Any]!

Converts the JavaScript value to an array.

func toDictionary() -> [AnyHashable : Any]!

Converts the JavaScript value to a dictionary.

func toPoint() -> CGPoint

Converts the value to a point structure.

func toRange() -> NSRange

Converts the value to a range.

func toRect() -> CGRect

Converts the value to a rectangle structure.

func toSize() -> CGSize

Converts the value to a size.

