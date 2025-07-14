

- Core Data
- NSDeleteRule
-  NSDeleteRule.denyDeleteRule 

Case

# NSDeleteRule.denyDeleteRule

A rule that prevents the deletion of the owning managed object if the relationship has references to other objects.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
case denyDeleteRule
```

## See Also

### Delete Rules

case noActionDeleteRule

A rule that prevents modification of the referenced managed objects.

case nullifyDeleteRule

A rule that nullifies the inverse relationship of the referenced managed objects.

case cascadeDeleteRule

A rule that deletes the referenced managed objects.

