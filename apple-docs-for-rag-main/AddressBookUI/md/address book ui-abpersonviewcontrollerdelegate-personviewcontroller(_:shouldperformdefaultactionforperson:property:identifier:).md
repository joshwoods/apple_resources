

- Address Book UI
- ABPersonViewControllerDelegate
-  personViewController(\_:shouldPerformDefaultActionForPerson:property:identifier:) 

Instance Method

# personViewController(\_:shouldPerformDefaultActionForPerson:property:identifier:)

Sent when the user selects a property value of the person displayed in a person view controller.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+

``` source
func personViewController(
    _ personViewController: ABPersonViewController,
    shouldPerformDefaultActionForPerson person: ABRecord,
    property: ABPropertyID,
    identifier: ABMultiValueIdentifier
) -> Bool
```

**Required**

## Parameters 

`personViewController`  

The sender.

`person`  

The person `personViewController` is displaying.

`property`  

The property whose value the user selected.

## Return Value

true if `personViewController` should perform its default action. Your application may quit as a result of this action. false: if `personViewController` should do nothing. The delegate may perform custom action processing.

