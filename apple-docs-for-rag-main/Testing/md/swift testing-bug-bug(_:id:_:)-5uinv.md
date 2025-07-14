

- Swift Testing
- Bug
-  bug(\_:id:\_:) 

Type Method

# bug(\_:id:\_:)

Construct a bug to track with a test.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
static func bug(
    _ url: String? = nil,
    id: String,
    _ title: Comment? = nil
) -> Self
```

Available when `Self` is `Bug`.

## Parameters 

`url`  

A URL referring to this bug in the associated bug-tracking system.

`id`  

The unique identifier of this bug in its associated bug-tracking system.

`title`  

Optionally, the human-readable title of the bug.

## Return Value

An instance of Bug representing the specified bug.

