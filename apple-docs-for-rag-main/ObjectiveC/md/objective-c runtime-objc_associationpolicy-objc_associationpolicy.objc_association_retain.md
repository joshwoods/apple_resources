

- Objective-C Runtime
- objc_AssociationPolicy
-  objc_AssociationPolicy.OBJC_ASSOCIATION_RETAIN 

Case

# objc_AssociationPolicy.OBJC_ASSOCIATION_RETAIN

Specifies a strong reference to the associated object, and that the association is made atomically.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
case OBJC_ASSOCIATION_RETAIN
```

## See Also

### Enumeration Cases

case OBJC_ASSOCIATION_ASSIGN

Specifies an unsafe unretained reference to the associated object.

case OBJC_ASSOCIATION_COPY

Specifies that the associated object is copied, and that the association is made atomically.

case OBJC_ASSOCIATION_COPY_NONATOMIC

Specifies that the associated object is copied, and that the association is not made atomically.

case OBJC_ASSOCIATION_RETAIN_NONATOMIC

Specifies a strong reference to the associated object, and that the association is not made atomically.

