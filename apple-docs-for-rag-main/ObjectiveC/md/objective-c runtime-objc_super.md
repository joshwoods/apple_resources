

- Objective-C Runtime
-  objc_super 

Structure

# objc_super

Specifies the superclass of an instance.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct objc_super
```

## Discussion

The compiler generates an `objc_super` data structure when it encounters the `super` keyword as the receiver of a message. It specifies the class definition of the particular superclass that should be messaged.

## Topics

### Fields

var receiver: Unmanaged&lt;AnyObject>

A pointer of type objc_object. Specifies an instance of a class.

var super_class: AnyClass

A pointer to a Class data structure. Specifies the particular superclass of the instance to message.

### Instance Properties

var receiver: Unmanaged&lt;AnyObject>

A pointer of type objc_object. Specifies an instance of a class.

var super_class: AnyClass

A pointer to a Class data structure. Specifies the particular superclass of the instance to message.

### Initializers

init(receiver: Unmanaged&lt;AnyObject>, super_class: AnyClass)

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Instance Data Types

struct objc_object

Represents an instance of a class.

