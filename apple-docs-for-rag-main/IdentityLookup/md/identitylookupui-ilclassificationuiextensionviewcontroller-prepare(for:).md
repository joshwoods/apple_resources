

- IdentityLookupUI
- ILClassificationUIExtensionViewController
-  prepare(for:) 

Instance Method

# prepare(for:)

Notifies the view controller just before the system presents it to the user.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+visionOS 1.0+

``` source
@MainActor
func prepare(for request: ILClassificationRequest)
```

## See Also

### Collecting Data from the User

func classificationResponse(for: ILClassificationRequest) -> ILClassificationResponse

Notifies the view controller when the user finishes entering data and presses the Done button.

