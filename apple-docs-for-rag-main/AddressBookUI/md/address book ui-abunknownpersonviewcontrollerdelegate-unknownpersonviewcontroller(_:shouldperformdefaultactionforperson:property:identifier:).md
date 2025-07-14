

- Address Book UI
- ABUnknownPersonViewControllerDelegate
-  unknownPersonViewController(\_:shouldPerformDefaultActionForPerson:property:identifier:) 

Instance Method

# unknownPersonViewController(\_:shouldPerformDefaultActionForPerson:property:identifier:)

Sent when the user selects a property value of the person displayed in a person view controller.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+

``` source
optional func unknownPersonViewController(
    _ personViewController: ABUnknownPersonViewController,
    shouldPerformDefaultActionForPerson person: ABRecord,
    property: ABPropertyID,
    identifier: ABMultiValueIdentifier
) -> Bool
```

## Parameters 

`person`  

The person `unknownPersonViewController` is displaying.

`property`  

The property whose value the user selected.

`identifier`  

The identifier for the value the user selected if `property` is a multivalue property; otherwise, `kABMultiValueInvalidIdentifier`.

## Return Value

true if `unknownPersonViewController` should perform its default action. Your application may quit as a result of this action. false: if `unknownPersonViewController` should do nothing. The delegate may perform custom action processing.

## See Also

### Responding to User Events

func unknownPersonViewController(ABUnknownPersonViewController, didResolveToPerson: ABRecord?)

Sent when the user finishes creating a contact or adding the displayed person properties to an existing contact.

**Required**

