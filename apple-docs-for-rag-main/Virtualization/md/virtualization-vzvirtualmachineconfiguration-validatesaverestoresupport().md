

- Virtualization
- VZVirtualMachineConfiguration
-  validateSaveRestoreSupport() 

Instance Method

# validateSaveRestoreSupport()

Determines whether the framework can save or restore the VM’s current configuration.

macOS 14.0+

``` source
func validateSaveRestoreSupport() throws
```

## Discussion

Use this method to verify that a virtual machine with this configuration is savable.

- Not all configuration options can be safely saved and restored from the configuration file on disk.

- If this method returns `false`, the caller should expect future calls to saveMachineStateTo(url:completionHandler:) to fail.

## See Also

### Validating the configuration

func validate() throws

Validates the current configuration settings and reports any issues that might prevent the successful initialization of the VM.

