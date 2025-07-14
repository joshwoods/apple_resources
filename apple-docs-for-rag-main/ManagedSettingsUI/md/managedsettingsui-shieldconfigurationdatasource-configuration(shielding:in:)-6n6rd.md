

- ManagedSettingsUI
- ShieldConfigurationDataSource
-  configuration(shielding:in:) 

Instance Method

# configuration(shielding:in:)

Requests a configuration to use for a shield that covers a website because of its category.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
func configuration(
    shielding webDomain: WebDomain,
    in category: ActivityCategory
) -> ShieldConfiguration
```

## Parameters 

`webDomain`  

The website that the shield covers.

`category`  

The category of the website that the shield covers.

## Return Value

The shield to display.

## See Also

### Styling a Website Shield

func configuration(shielding: WebDomain) -> ShieldConfiguration

Requests a configuration to use for a shield that covers a website.

