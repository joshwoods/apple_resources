

- JavaScriptCore
- JSValue
-  toRange() 

Instance Method

# toRange()

Converts the value to a range.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func toRange() -> NSRange
```

## Return Value

A range representation of the value.

## Discussion

This method treats the value as a JavaScript object, reading the values of its `location` and `length` properties using the toDouble() method and creating a NSRange structure from the result. If the value is not a JavaScript object or does not have the appropriate properties, the resulting range is invalid.

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

func toString() -> String!

Converts the JavaScript value to a native string.

func toDate() -> Date!

Converts the JavaScript value to a date object.

func toArray() -> [Any]!

Converts the JavaScript value to an array.

func toDictionary() -> [AnyHashable : Any]!

Converts the JavaScript value to a dictionary.

func toPoint() -> CGPoint

Converts the value to a point structure.

func toRect() -> CGRect

Converts the value to a rectangle structure.

func toSize() -> CGSize

Converts the value to a size.

