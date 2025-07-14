

- XCUIAutomation
- XCUIGestureVelocity
-  XCUIGestureVelocity.FloatLiteralType 

Type Alias

# XCUIGestureVelocity.FloatLiteralType

The native type that specifies the gesture velocity value.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSXcode 16.3+

``` source
typealias FloatLiteralType = CGFloat.NativeType
```

## Discussion

The native type that specifies the gesture velocity value is `Float` on 32-bit architectures and `Double` on 64-bit architectures.

## See Also

### Creating a gesture velocity

init(CGFloat)

Creates a gesture velocity, expressed as a float.

init(integerLiteral: Int)

Creates a gesture velocity with an integer value.

init(floatLiteral: XCUIGestureVelocity.FloatLiteralType)

Creates a gesture velocity with a float value.

init(rawValue: CGFloat)

Creates a gesture velocity with a raw value, expressed as a float.

typealias IntegerLiteralType

A type that specifies a gesture velocity with an integer literal.

