

- ManagedSettingsUI
- ShieldConfigurationDataSource
-  configuration(shielding:) 

Instance Method

# configuration(shielding:)

Requests a configuration to use for a shield that covers a website.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
func configuration(shielding webDomain: WebDomain) -> ShieldConfiguration
```

## Parameters 

`webDomain`  

The website that the shield covers.

## Return Value

The shield to display.

## See Also

### Styling a Website Shield

func configuration(shielding: WebDomain, in: ActivityCategory) -> ShieldConfiguration

Requests a configuration to use for a shield that covers a website because of its category.

