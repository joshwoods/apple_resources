

- JavaScriptCore
- JSValue
-  toArray() 

Instance Method

# toArray()

Converts the JavaScript value to an array.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
func toArray() -> [Any]!
```

## Return Value

The array representation of the value.

## Discussion

If the value is a JavaScript object, this method reads the object’s `length` property as an unsigned integer, creates an NSArray object of the corresponding size, and recursively copies and converts any properties corresponding to indices within the array bounds. JavaScript converts each element to a native object using the rules listed in Convert Between JavaScript and Native Types.

This method returns `nil` if the JavaScript value is `null` or `undefined`, and throws a JavaScript `TypeError` if the value is not a JavaScript object.

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

