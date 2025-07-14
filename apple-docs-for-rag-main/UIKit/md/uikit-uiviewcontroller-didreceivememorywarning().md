

- UIKit
- UIViewController
-  didReceiveMemoryWarning() 

Instance Method

# didReceiveMemoryWarning()

Sent to the view controller when the app receives a memory warning.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func didReceiveMemoryWarning()
```

## Mentioned in 

Responding to memory warnings

## Discussion

Your app never calls this method directly. Instead, this method is called when the system determines that the amount of available memory is low.

You can override this method to release any additional memory used by your view controller. If you do, your implementation of this method must call the `super` implementation at some point.

