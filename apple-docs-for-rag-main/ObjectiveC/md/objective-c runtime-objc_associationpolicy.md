

- Objective-C Runtime
-  objc_AssociationPolicy 

Enumeration

# objc_AssociationPolicy

Type to specify the behavior of an association.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum objc_AssociationPolicy
```

## Topics

### Enumeration Cases

case OBJC_ASSOCIATION_ASSIGN

Specifies an unsafe unretained reference to the associated object.

case OBJC_ASSOCIATION_COPY

Specifies that the associated object is copied, and that the association is made atomically.

case OBJC_ASSOCIATION_COPY_NONATOMIC

Specifies that the associated object is copied, and that the association is not made atomically.

case OBJC_ASSOCIATION_RETAIN

Specifies a strong reference to the associated object, and that the association is made atomically.

case OBJC_ASSOCIATION_RETAIN_NONATOMIC

Specifies a strong reference to the associated object, and that the association is not made atomically.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

