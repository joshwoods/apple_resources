

- PassKit (Apple Pay and Wallet)
- PKPass
-  init(data:) 

Initializer

# init(data:)

Creates a pass using the data you provide.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
init(data: Data) throws
```

## Parameters 

`data`  

A signed pass.

## Discussion

If there’s a problem encoding the data you supply, this method sets the `error` parameter based on the type of problem:

- The pass contains invalid data—this method throws the PKPassKitError.Code.invalidDataError error.

- The signature of the pass is invalid—this method throws the PKPassKitError.Code.invalidSignature error.

- For other types of errors, `/PassKit/PKPassKitError/localizedDescription` contains a string suitable for presentation to the user.

Check the console for more detailed information.

