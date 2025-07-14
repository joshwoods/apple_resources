

- ManagedSettingsUI
- ShieldConfigurationDataSource
-  configuration(shielding:in:) 

Instance Method

# configuration(shielding:in:)

Requests a configuration to use for a shield that covers an application because of its category.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
func configuration(
    shielding application: Application,
    in category: ActivityCategory
) -> ShieldConfiguration
```

## Parameters 

`application`  

The application the shield covers.

`category`  

The category of the application that the shield covers.

## Return Value

The shield to display.

## See Also

### Styling an Application Shield

func configuration(shielding: Application) -> ShieldConfiguration

Requests a configuration to use for a shield that covers an application.

