

- UIKit
- UIView
- UIView.Invalidating
-  init(wrappedValue:\_:\_:\_:\_:\_:\_:) 

Initializer

# init(wrappedValue:\_:\_:\_:\_:\_:\_:)

Creates a property wrapper that notifies the system when a change in the property value invalidates aspects of the containing view.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOSSwift 5.1+

``` source
init(
    wrappedValue: Value,
    _ invalidation1: InvalidationType1,
    _ invalidation2: InvalidationType2,
    _ invalidation3: InvalidationType3,
    _ invalidation4: InvalidationType4,
    _ invalidation5: InvalidationType5,
    _ invalidation6: InvalidationType6
) where InvalidationType == UIView.Invalidations.Tuple, UIView.Invalidations.Tuple>, UIView.Invalidations.Tuple>, InvalidationType1 : UIViewInvalidating, InvalidationType2 : UIViewInvalidating, InvalidationType3 : UIViewInvalidating, InvalidationType4 : UIViewInvalidating, InvalidationType5 : UIViewInvalidating, InvalidationType6 : UIViewInvalidating
```

## Parameters 

`wrappedValue`  

The underlying value referenced by the invalidating variable.

`invalidation1`  

A type of invalidation.

`invalidation2`  

A type of invalidation.

`invalidation3`  

A type of invalidation.

`invalidation4`  

A type of invalidation.

`invalidation5`  

A type of invalidation.

`invalidation6`  

A type of invalidation.

## See Also

### Creating an Invalidating Property Wrapper

init(wrappedValue: Value, InvalidationType)

Creates a property wrapper that notifies the system when a change in the property value invalidates an aspect of the containing view.

init&lt;InvalidationType1, InvalidationType2>(wrappedValue: Value, InvalidationType1, InvalidationType2)

Creates a property wrapper that notifies the system when a change in the property value invalidates aspects of the containing view.

init&lt;InvalidationType1, InvalidationType2, InvalidationType3>(wrappedValue: Value, InvalidationType1, InvalidationType2, InvalidationType3)

Creates a property wrapper that notifies the system when a change in the property value invalidates aspects of the containing view.

init&lt;InvalidationType1, InvalidationType2, InvalidationType3, InvalidationType4>(wrappedValue: Value, InvalidationType1, InvalidationType2, InvalidationType3, InvalidationType4)

Creates a property wrapper that notifies the system when a change in the property value invalidates aspects of the containing view.

init&lt;InvalidationType1, InvalidationType2, InvalidationType3, InvalidationType4, InvalidationType5>(wrappedValue: Value, InvalidationType1, InvalidationType2, InvalidationType3, InvalidationType4, InvalidationType5)

Creates a property wrapper that notifies the system when a change in the property value invalidates aspects of the containing view.

init&lt;InvalidationType1, InvalidationType2, InvalidationType3, InvalidationType4, InvalidationType5, InvalidationType6, InvalidationType7>(wrappedValue: Value, InvalidationType1, InvalidationType2, InvalidationType3, InvalidationType4, InvalidationType5, InvalidationType6, InvalidationType7)

Creates a property wrapper that notifies the system when a change in the property value invalidates aspects of the containing view.

init&lt;InvalidationType1, InvalidationType2, InvalidationType3, InvalidationType4, InvalidationType5, InvalidationType6, InvalidationType7, InvalidationType8>(wrappedValue: Value, InvalidationType1, InvalidationType2, InvalidationType3, InvalidationType4, InvalidationType5, InvalidationType6, InvalidationType7, InvalidationType8)

Creates a property wrapper that notifies the system when a change in the property value invalidates aspects of the containing view.

init&lt;InvalidationType1, InvalidationType2, InvalidationType3, InvalidationType4, InvalidationType5, InvalidationType6, InvalidationType7, InvalidationType8, InvalidationType9>(wrappedValue: Value, InvalidationType1, InvalidationType2, InvalidationType3, InvalidationType4, InvalidationType5, InvalidationType6, InvalidationType7, InvalidationType8, InvalidationType9)

Creates a property wrapper that notifies the system when a change in the property value invalidates aspects of the containing view.

init&lt;InvalidationType1, InvalidationType2, InvalidationType3, InvalidationType4, InvalidationType5, InvalidationType6, InvalidationType7, InvalidationType8, InvalidationType9, InvalidationType10>(wrappedValue: Value, InvalidationType1, InvalidationType2, InvalidationType3, InvalidationType4, InvalidationType5, InvalidationType6, InvalidationType7, InvalidationType8, InvalidationType9, InvalidationType10)

Creates a property wrapper that notifies the system when a change in the property value invalidates aspects of the containing view.

