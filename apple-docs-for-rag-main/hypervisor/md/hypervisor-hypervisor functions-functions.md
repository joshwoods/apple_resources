

- Hypervisor
-  Hypervisor Functions 

API Collection

# Hypervisor Functions

## Topics

### Functions

func hv_sme_config_get_max_svl_bytes(UnsafeMutablePointer&lt;Int>) -> hv_return_t

func hv_vcpu_apic_ctrl(hv_vcpuid_t, hv_apic_ctrl_t) -> hv_return_t

func hv_vcpu_apic_get_state(hv_vcpuid_t, UnsafeMutablePointer&lt;hv_apic_state_ext_t>) -> hv_return_t

func hv_vcpu_apic_lsc_enter_imm32(hv_vcpuid_t, UInt64, UInt32, UInt16, UInt32, UnsafeMutablePointer&lt;UInt64>?, UInt32) -> hv_return_t

func hv_vcpu_apic_lsc_enter_r32(hv_vcpuid_t, Bool, UInt64, UInt32, UInt16, hv_x86_reg_t, UnsafeMutablePointer&lt;UInt64>?, UInt32) -> hv_return_t

func hv_vcpu_apic_lsc_invalidate(hv_vcpuid_t) -> hv_return_t

func hv_vcpu_apic_put_state(hv_vcpuid_t, UnsafePointer&lt;hv_apic_state_ext_t>) -> hv_return_t

func hv_vcpu_apic_read(hv_vcpuid_t, UInt32, UnsafeMutablePointer&lt;UInt32>) -> hv_return_t

func hv_vcpu_apic_trigger_lvt(hv_vcpuid_t, hv_apic_lvt_flavor_t) -> hv_return_t

func hv_vcpu_apic_write(hv_vcpuid_t, UInt32, UInt32, UnsafeMutablePointer&lt;Bool>) -> hv_return_t

func hv_vcpu_exit_apic_access_read(hv_vcpuid_t, UnsafeMutablePointer&lt;UInt32>) -> hv_return_t

func hv_vcpu_exit_info(hv_vcpuid_t, UnsafeMutablePointer&lt;hv_vm_exitinfo_t>) -> hv_return_t

func hv_vcpu_exit_init_ap(hv_vcpuid_t, UnsafeMutablePointer&lt;Bool>, UInt32) -> hv_return_t

func hv_vcpu_exit_inject_excp(hv_vcpuid_t, UnsafeMutablePointer&lt;UInt8>, UnsafeMutablePointer&lt;Bool>, UnsafeMutablePointer&lt;UInt32>, UnsafeMutablePointer&lt;Bool>) -> hv_return_t

func hv_vcpu_exit_ioapic_eoi(hv_vcpuid_t, UnsafeMutablePointer&lt;UInt8>) -> hv_return_t

func hv_vcpu_exit_startup_ap(hv_vcpuid_t, UnsafeMutablePointer&lt;Bool>, UInt32, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

func hv_vcpu_get_idle_time(hv_vcpuid_t, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

func hv_vcpu_get_sme_p_reg(hv_vcpu_t, hv_sme_p_reg_t, UnsafeMutablePointer&lt;UInt8>, Int) -> hv_return_t

Returns the value of a vCPU P predicate register in streaming Scalable Vector Extension (SVE) mode.

func hv_vcpu_get_sme_state(hv_vcpu_t, UnsafeMutablePointer&lt;hv_vcpu_sme_state_t>) -> hv_return_t

Gets the current Scalable Matrix Extension (SME) state.

func hv_vcpu_get_sme_z_reg(hv_vcpu_t, hv_sme_z_reg_t, UnsafeMutablePointer&lt;UInt8>, Int) -> hv_return_t

Returns the value of a vCPU Z vector register in streaming Scalable Vector Extension (SVE) mode.

func hv_vcpu_get_sme_za_reg(hv_vcpu_t, UnsafeMutablePointer&lt;UInt8>, Int) -> hv_return_t

Returns the value of the vCPU ZA matrix register in streaming Scalable Vector Extension (SVE) mode.

func hv_vcpu_get_sme_zt0_reg(hv_vcpu_t, UnsafeMutablePointer&lt;hv_sme_zt0_uchar64_t>) -> hv_return_t

Returns the current value of the vCPU ZT0 register in streaming Scalable Vector Extension (SVE) mode.

func hv_vcpu_inject_extint(hv_vcpuid_t) -> hv_return_t

func hv_vcpu_set_sme_p_reg(hv_vcpu_t, hv_sme_p_reg_t, UnsafePointer&lt;UInt8>, Int) -> hv_return_t

Sets the value of a vCPU P predicate register in streaming Scalable Vector Extension (SVE) mode.

func hv_vcpu_set_sme_state(hv_vcpu_t, UnsafePointer&lt;hv_vcpu_sme_state_t>) -> hv_return_t

Sets the SME state consisting of the streaming Scalable Vector Extension (SVE) mode and ZA storage enable.

func hv_vcpu_set_sme_z_reg(hv_vcpu_t, hv_sme_z_reg_t, UnsafePointer&lt;UInt8>, Int) -> hv_return_t

Sets the value of a vCPU Z vector register in streaming Scalable Vector Extension (SVE) mode.

func hv_vcpu_set_sme_za_reg(hv_vcpu_t, UnsafePointer&lt;UInt8>, Int) -> hv_return_t

Sets the value of the vCPU ZA matrix register in streaming Scalable Vector Extension (SVE) mode.

func hv_vcpu_set_sme_zt0_reg(hv_vcpu_t, UnsafePointer&lt;hv_sme_zt0_uchar64_t>) -> hv_return_t

Sets the value of the vCPU ZT0 register in streaming Scalable Vector Extension (SVE) mode.

func hv_vcpu_vmx_status(hv_vcpuid_t, UnsafeMutablePointer&lt;UInt32>) -> hv_return_t

func hv_vm_allocate(UnsafeMutablePointer&lt;UnsafeMutableRawPointer?>, Int, hv_allocate_flags_t) -> hv_return_t

func hv_vm_atpic_assert_irq(Int32) -> hv_return_t

func hv_vm_atpic_deassert_irq(Int32) -> hv_return_t

func hv_vm_atpic_get_state(UnsafeMutablePointer&lt;hv_atpic_state_ext_t>, Bool) -> hv_return_t

func hv_vm_atpic_port_read(Int32, UnsafeMutablePointer&lt;UInt8>) -> hv_return_t

func hv_vm_atpic_port_write(Int32, UInt8) -> hv_return_t

func hv_vm_atpic_put_state(UnsafePointer&lt;hv_atpic_state_ext_t>, Bool) -> hv_return_t

func hv_vm_config_get_default_ipa_size(UnsafeMutablePointer&lt;UInt32>) -> hv_return_t

func hv_vm_config_get_ipa_size(hv_vm_config_t, UnsafeMutablePointer&lt;UInt32>) -> hv_return_t

func hv_vm_config_get_max_ipa_size(UnsafeMutablePointer&lt;UInt32>) -> hv_return_t

func hv_vm_config_set_ipa_size(hv_vm_config_t, UInt32) -> hv_return_t

func hv_vm_deallocate(UnsafeMutableRawPointer, Int) -> hv_return_t

func hv_vm_ioapic_assert_irq(Int32) -> hv_return_t

func hv_vm_ioapic_deassert_irq(Int32) -> hv_return_t

func hv_vm_ioapic_get_state(UnsafeMutablePointer&lt;hv_ioapic_state_ext_t>) -> hv_return_t

func hv_vm_ioapic_pulse_irq(Int32) -> hv_return_t

func hv_vm_ioapic_put_state(UnsafePointer&lt;hv_ioapic_state_ext_t>) -> hv_return_t

func hv_vm_ioapic_read(hv_gpaddr_t, UnsafeMutablePointer&lt;UInt32>) -> hv_return_t

func hv_vm_ioapic_write(hv_gpaddr_t, UInt32) -> hv_return_t

func hv_vm_lapic_msi(UInt64, UInt64) -> hv_return_t

func hv_vm_lapic_set_intr(hv_vcpuid_t, UInt8, hv_apic_intr_trigger_t) -> hv_return_t

func hv_vm_map_space(hv_vm_space_t, hv_uvaddr_t, hv_gpaddr_t, Int, hv_memory_flags_t) -> hv_return_t

Maps a region in the virtual address space of the current task into a guest physical address space of the VM.

func hv_vm_protect_space(hv_vm_space_t, hv_gpaddr_t, Int, hv_memory_flags_t) -> hv_return_t

Modifies the permissions of a region in a guest physical address space of the VM.

func hv_vm_send_ioapic_intr(UInt64) -> hv_return_t

func hv_vm_set_apic_bus_freq(UInt64) -> hv_return_t

func hv_vm_space_create(UnsafeMutablePointer&lt;hv_vm_space_t>) -> hv_return_t

Creates an additional guest address space for the current task.

func hv_vm_space_destroy(hv_vm_space_t) -> hv_return_t

Destroys the address space instance associated with the current task.

func hv_vm_unmap_space(hv_vm_space_t, hv_gpaddr_t, Int) -> hv_return_t

Umaps a region in a guest physical address space of the VM.

func hv_vmx_vcpu_set_apic_address_space(hv_vcpuid_t, hv_vm_space_t, hv_gpaddr_t) -> hv_return_t

## See Also

### Reference

Hypervisor Structures

Hypervisor Constants

Hypervisor Data Types

