

- Objective-C Runtime
-  objc_object 

Structure

# objc_object

Represents an instance of a class.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct objc_object
```

## Topics

### Initializers

init(isa: AnyClass)

### Instance Properties

var isa: AnyClass

A pointer to the class definition of which this object is an instance.

Deprecated

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Instance Data Types

struct objc_super

Specifies the superclass of an instance.

