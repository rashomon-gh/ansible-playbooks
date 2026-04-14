# opensuse-leap

openSUSE Leap post installation steps automated with ansible.

## playbooks

> [!NOTE]
> If you don't need specific playbooks you can comment them out in the `playbook.yml` file.

The directory contains a set of ansible playbooks for setting up some preferred applications after setup.

## what's not covered

| Topic | Reason |
|---|---|
| CUDA Toolkit installation | Check [Nvidia CUDA Toolkit Downloads](https://developer.nvidia.com/cuda-downloads) and follow openSUSE-specific instructions. Ensure you install a compatible gcc compiler version. |
| Secure Boot Setup | Check openSUSE documentation and your motherboard manual for Secure Boot configuration with Linux. |
| Gnome shell extensions | Install based on your preferences using Extension Manager or browser extensions. |
| VPNs and other email clients | Install based on your personal preferences and requirements. |

> [!TIP]
> If you're using a new gen Thinkpad (e.g. P1 Gen 7 or newer), read the [OMGLinux guide](https://www.omglinux.com/boot-linux-modern-lenovo-thinkpads-bios-setting/) on how to enable secure boot for non-Microsoft operating systems in the bios.

> [!TIP]
> openSUSE uses zypper as package manager. For more information, check the [openSUSE documentation](https://en.opensuse.org/Portal:Zypper).

> [!TIP]
> If you've a dual gpu laptop (iGPU+dGPU), use the following as the launcher command to run games on the dGPU: `__NV_PRIME_RENDER_OFFLOAD=1 __GLX_VENDOR_LIBRARY_NAME=nvidia %command%` if games run on iGPU by default.
