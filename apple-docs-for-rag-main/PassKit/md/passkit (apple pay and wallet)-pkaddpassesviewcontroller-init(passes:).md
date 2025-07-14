

- PassKit (Apple Pay and Wallet)
- PKAddPassesViewController
-  init(passes:) 

Initializer

# init(passes:)

Initializes and returns a newly created add-passes view controller with an array of passes.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
init?(passes: [PKPass])
```

## Parameters 

`passes`  

The passes for the view controller to display.

## Return Value

The initialized add-passes view controller object or `nil` if there was a problem initializing the object.

## See Also

### Creating an add-passes view controller

init?(pass: PKPass)

Initializes and returns a newly created add-passes view controller with a single pass.

init(issuerData: Data, signature: Data) throws

Initializes and returns a new add-passes view controller with the issuer data, and signature you provide.

