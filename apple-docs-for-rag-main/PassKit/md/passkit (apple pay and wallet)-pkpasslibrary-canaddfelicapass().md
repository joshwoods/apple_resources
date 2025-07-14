

- PassKit (Apple Pay and Wallet)
- PKPassLibrary
-  canAddFelicaPass() 

Instance Method

# canAddFelicaPass()

Returns a Boolean value that indicates whether the library can add FeliCa™ passes.

iOS 10.1+iPadOS 10.1+Mac Catalyst 13.1+macOS 10.12+visionOS 1.0+watchOS 3.1+

``` source
func canAddFelicaPass() -> Bool
```

## Discussion

By default, this method returns false.

## See Also

### Adding passes

func canAddSecureElementPass(primaryAccountIdentifier: String) -> Bool

Returns a Boolean value that indicates whether PassKit can add a Secure Element pass for the specified account.

func addPasses([PKPass], withCompletionHandler: ((PKPassLibraryAddPassesStatus) -> Void)?)

Presents a user interface for adding multiple passes at once.

enum PKPassLibraryAddPassesStatus

Statuses that PassKit uses when it adds passes to the pass library.

