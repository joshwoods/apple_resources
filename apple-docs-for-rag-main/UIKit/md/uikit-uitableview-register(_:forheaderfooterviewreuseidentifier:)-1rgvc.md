

- UIKit
- UITableView
-  register(\_:forHeaderFooterViewReuseIdentifier:) 

Instance Method

# register(\_:forHeaderFooterViewReuseIdentifier:)

Registers a nib object that contains a header or footer with the table view under a specified identifier.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0–1.0Deprecated

``` source
@MainActor
func register(
    _ nib: UINib?,
    forHeaderFooterViewReuseIdentifier identifier: String
)
```

## Parameters 

`nib`  

A nib object that specifies the nib file to use to create the header or footer view. This parameter can’t be `nil`.

`identifier`  

The reuse identifier for the header or footer view. This parameter must not be `nil` and must not be an empty string.

## Discussion

Before dequeueing any header or footer views, call this method or the register(_:forHeaderFooterViewReuseIdentifier:) method to tell the table view how to create new instances of your views. If a view of the specified type isn’t currently in a reuse queue, the table view uses the provided information to create a new one automatically.

If you previously registered a class or nib file with the same reuse identifier, the nib you specify in the `nib` parameter replaces the old entry. You may specify `nil` for `nib` if you want to unregister the nib from the specified reuse identifier.

## See Also

### Recycling section headers and footers

func register(AnyClass?, forHeaderFooterViewReuseIdentifier: String)

Registers a class to use in creating new table header or footer views.

func dequeueReusableHeaderFooterView(withIdentifier: String) -> UITableViewHeaderFooterView?

Returns a reusable header or footer view after locating it by its identifier.

