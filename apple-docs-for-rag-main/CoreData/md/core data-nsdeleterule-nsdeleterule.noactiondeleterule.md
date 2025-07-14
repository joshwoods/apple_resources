

- Core Data
- NSDeleteRule
-  NSDeleteRule.noActionDeleteRule 

Case

# NSDeleteRule.noActionDeleteRule

A rule that prevents modification of the referenced managed objects.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
case noActionDeleteRule
```

## Discussion

If you use this delete rule, make sure you delete any referenced managed objects or nullify their inverse relationships. Otherwise, those objects will reference an object that doesn’t exist, and your persistent store will be in an inconsistent state.

## See Also

### Delete Rules

case nullifyDeleteRule

A rule that nullifies the inverse relationship of the referenced managed objects.

case cascadeDeleteRule

A rule that deletes the referenced managed objects.

case denyDeleteRule

A rule that prevents the deletion of the owning managed object if the relationship has references to other objects.

