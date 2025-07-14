

- PassKit (Apple Pay and Wallet)
- PKPassLibrary
-  canAddSecureElementPass(primaryAccountIdentifier:) 

Instance Method

# canAddSecureElementPass(primaryAccountIdentifier:)

Returns a Boolean value that indicates whether PassKit can add a Secure Element pass for the specified account.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOS 10.12+visionOS 1.0+watchOS 6.2+

``` source
func canAddSecureElementPass(primaryAccountIdentifier: String) -> Bool
```

## Parameters 

`primaryAccountIdentifier`  

A unique identifer for the underlying primary account number (PAN) for funding transactions. This isn’t the PAN itself.

## Return Value

true if PassKit can add a secure element pass for the specified account; otherwise, false.

## Discussion

Adding a Secure Element pass requires a special entitlement that Apple provides. If the entitlement isn’t present, this method returns false.

## See Also

### Adding passes

func canAddFelicaPass() -> Bool

Returns a Boolean value that indicates whether the library can add FeliCa™ passes.

func addPasses([PKPass], withCompletionHandler: ((PKPassLibraryAddPassesStatus) -> Void)?)

Presents a user interface for adding multiple passes at once.

enum PKPassLibraryAddPassesStatus

Statuses that PassKit uses when it adds passes to the pass library.

