

- UIKit
- UIStoryboardSegue
-  init(identifier:source:destination:performHandler:) 

Initializer

# init(identifier:source:destination:performHandler:)

Creates a segue that calls a block to perform the segue transition.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0–1.0Deprecated

``` source
@MainActor
convenience init(
    identifier: String?,
    source: UIViewController,
    destination: UIViewController,
    performHandler: @escaping () -> Void
)
```

## Parameters 

`identifier`  

The identifier you want to associate with this particular instance of the segue. You can use this identifier to differentiate one type of segue from another at runtime.

`source`  

The view controller visible at the start of the segue.

`destination`  

The view controller to display after the completion of the segue.

`performHandler`  

A block to be called when the segue’s perform() method is called.

## Return Value

An initialized segue object.

## Discussion

You use this method as an alternative to creating a subclass. Your perform handler should do all of the work necessary to transition between the source and destination view controllers, exactly as if you were implementing the perform() method.

## See Also

### Related Documentation

func perform()

Performs the visual transition for the segue.

