

- ProximityReader
- PaymentCardReader
-  init(options:) 

Initializer

# init(options:)

Creates a payment card reader with the specified options.

iOS 15.4+iPadOS 15.4+Mac Catalyst 17.0+

``` source
init(options: PaymentCardReader.Options = .init())
```

## Parameters 

`options`  

The configuration settings for the reader.

## Discussion

Keep a strong reference to the returned object for the duration of the reader session.

## See Also

### Creating a payment reader

struct Options

Additional information you use to configure a payment card reader.

