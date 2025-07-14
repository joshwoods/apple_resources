

- StoreKit
- SKArcadeService
-  registerArcadeAppWithRandom(fromLib:randomFromLibLength:resultHandler:) 

Type Method

# registerArcadeAppWithRandom(fromLib:randomFromLibLength:resultHandler:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func registerArcadeAppWithRandom(
    fromLib randomFromLib: Data,
    randomFromLibLength: UInt32,
    resultHandler: @escaping (Data?, UInt32, Data?, UInt32, (any Error)?) -> Void
)
```

