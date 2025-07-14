

- JavaScriptCore
- JSValue
-  toObjectOf(\_:) 

Instance Method

# toObjectOf(\_:)

Converts the JavaScript value to a native object of the specified class.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
func toObjectOf(_ expectedClass: AnyClass!) -> Any!
```

## Parameters 

`expectedClass`  

The Objective-C or Swift class type to convert the value to.

## Return Value

An Objective-C or Swift object representing the JavaScript value, or `nil` if the value cannot be converted to the expected class.

## Discussion

Use this method to enforce a specific type conversion from JavaScript, or to retrieve Objective-C or Swift objects of custom classes that were bridged into JavaScript using the JSExport protocol.

## See Also

### Reading and Converting JavaScript Values

func toObject() -> Any!

Converts the JavaScript value to a native object.

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

func toRange() -> NSRange

Converts the value to a range.

func toRect() -> CGRect

Converts the value to a rectangle structure.

func toSize() -> CGSize

Converts the value to a size.

