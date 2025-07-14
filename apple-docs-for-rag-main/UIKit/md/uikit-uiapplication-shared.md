

- UIKit
- UIApplication
-  shared 

Type Property

# shared

The singleton app instance.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class var shared: UIApplication { get }
```

## Return Value

The app instance is created in the UIApplicationMain(_:_:_:_:) function.

## Discussion

The UIApplicationMain(_:_:_:_:) function creates the shared app instance at launch time.

