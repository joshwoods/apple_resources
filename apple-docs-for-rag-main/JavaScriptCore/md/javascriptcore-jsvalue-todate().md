

- JavaScriptCore
- JSValue
-  toDate() 

Instance Method

# toDate()

Converts the JavaScript value to a date object.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
func toDate() -> Date!
```

## Return Value

The date representation of the value.

## Discussion

If the value contains a JavaScript `Date` object, this method returns an equivalent NSDate representation. Otherwise, this method uses JavaScript type coercion to interpret the value as a number of seconds and creates an NSDate object with the dateWithTimeIntervalSince1970: method.

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

