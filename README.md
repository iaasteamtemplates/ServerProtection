# ServerProtection
IaaS Server or Endpoint protection scripts

This is a simple Cloud-init compatible version of our Linux Server Protection installation script.

Since cloud-init is becoming a big part of automating the post-deployment stage of a machine (and because Azure supports it on all the marketplace OS images for Linux) I recently sat down and built this to help make my testing easier.

What is does is very simple, and on par with what the script we have in the KB does; Essentially it instructs cloud-init to use the platform’s package manager to install a few packages, then run three commands (wget to download the Sophos installer, chmod to set the execute bit, and then run SophosInstaller).
