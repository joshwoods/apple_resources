

- UIKit
- UINib
- UINib.OptionsKey
-  externalObjects 

Type Property

# externalObjects

The replacements for any proxy objects in the nib file.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
static let externalObjects: UINib.OptionsKey
```

## Discussion

The value for this key is an NSDictionary object. The keys of the dictionary are the names of any proxy objects in the nib file, and the value for each key is the actual object to use in place of the proxy.

