

- IdentityLookupUI
- ILClassificationUIExtensionViewController
-  classificationResponse(for:) 

Instance Method

# classificationResponse(for:)

Notifies the view controller when the user finishes entering data and presses the Done button.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+visionOS 1.0+

``` source
@MainActor
func classificationResponse(for request: ILClassificationRequest) -> ILClassificationResponse
```

## See Also

### Collecting Data from the User

func prepare(for: ILClassificationRequest)

Notifies the view controller just before the system presents it to the user.

