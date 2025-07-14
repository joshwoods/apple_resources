

- ManagedSettingsUI
- ShieldConfigurationDataSource
-  configuration(shielding:) 

Instance Method

# configuration(shielding:)

Requests a configuration to use for a shield that covers an application.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
func configuration(shielding application: Application) -> ShieldConfiguration
```

## Parameters 

`application`  

The application the shield covers.

## Return Value

The shield to display.

## See Also

### Styling an Application Shield

func configuration(shielding: Application, in: ActivityCategory) -> ShieldConfiguration

Requests a configuration to use for a shield that covers an application because of its category.

