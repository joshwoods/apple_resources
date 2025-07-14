

- Create ML
- MLDataValueConvertible
-  dataValueType 

Type Property

# dataValueType

The underlying type the conforming type uses when it wraps itself in a data value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
static var dataValueType: MLDataValue.ValueType { get }
```

**Required**

## Discussion

See MLDataValue.ValueType for a list of available options.

## See Also

### Converting from a type’s instance to a data value

var dataValue: MLDataValue

The value of the conforming type’s instance wrapped in a data value.

**Required**

