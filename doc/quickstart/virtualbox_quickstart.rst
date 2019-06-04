:Author: OSGeoLive
:Author: Cameron Shorter
:Version: osgeolive4.0
:License: Creative Commons Attribution-ShareAlike 3.0 Unported  (CC BY-SA 3.0)

********************************************************************************
OSGeoLive Quickstart for Virtual Box
********************************************************************************

Here we describe a method for running an OSGeoLive DVD or ISO in the `VirtualBox <http://www.virtualbox.org/>`_ Virtual Machine.

VirtualBox is an Open Source Virtual Machine which is used by many of the OSGeoLive developers and testers.

System Requirements
--------------------------------------------------------------------------------

* RAM: 1 GB, preferably 2 GB if you plan to run other applications as well
* Spare Hard Disk Space:

 * |osgeolive-hdspace| if running from ISO
 * 17 GB if installing locally from an ISO

Create a Virtual Machine
--------------------------------------------------------------------------------
Download and install `Virtual Box <http://www.virtualbox.org/>`_. On Debian/Ubuntu Linux do the following:

  ``apt-get install virtualbox-ose``


Open Virtual Box 

  .. image:: /images/projects/virtualization/virtualbox.png
    :scale: 70 %

Select :guilabel:`New` to create a new Virtual Machine.

  .. image:: /images/projects/virtualization/virtualbox_create_vm.png
    :scale: 70 %

Select :guilabel:`Next`

  .. image:: /images/projects/virtualization/virtualbox_select_name.png
    :scale: 70 %

Set a name for the image, and select "Linux", "Ubuntu".

  .. image:: /images/projects/virtualization/virtualbox_memory.png
    :scale: 70 %

Set Base Memory to at least 768 MB, 1 GB is better for trialing java based applications.

  .. image:: /images/projects/virtualization/virtualbox_no_hard_disk.png
    :scale: 70 %

Simple install: Deselect "Boot Hard Disk", the Virtual Machine will always
boot from an simulated DVD.

If you wish to have a persistent virtual machine, which stores state
between sessions and which can have improved screen resolution settings
and tools set, then include the hard disk, and install later.

  .. image:: /images/projects/virtualization/virtualbox_warning_no_hard_disk.png
    :scale: 70 %

Select :guilabel:`Continue`

  .. image:: /images/projects/virtualization/virtualbox_final_check.png
    :scale: 70 %

Select :guilabel:`Finish`

  .. image:: /images/projects/virtualization/virtualbox_select_settings.png
    :scale: 70 %

The image is now created, but we now need to simulate having an OSGeoLive DVD in the CD drive.

Right click on the "osgeolive" image, and select :guilabel:`Settings`.

  .. image:: /images/projects/virtualization/virtualbox_set_cd.png
    :scale: 70 %

Select "Storage", CD/DVD Device, ...

  .. image:: /images/projects/virtualization/virtualbox_add_dvd.png
    :scale: 70 %

Select the OSGeoLive image.

  .. image:: /images/projects/virtualization/virtualbox_start_vm.png
    :scale: 70 %

Now you can start the virtual machine as per the :doc:`osgeolive_quickstart`

Create permanent Virtual Machine
--------------------------------------------------------------------------------
If you plan to use the OSGeoLive DVD a lot, you will likey want to create a permanent virtual machine, as per: :doc:`osgeolive_install_quickstart`.

Increase Display Size
--------------------------------------------------------------------------------
You can then add the virtual boots tools which support higher screen
resolution support, copy and paste between guest and host, graphics
acceleration, and more.

Make sure you're computer is connected to the internet.

  .. image:: /images/projects/virtualization/virtualbox_synaptic_menu.png
    :scale: 70 %

Select the synaptic package manager application.

Enter password = "user"

  .. image:: /images/projects/virtualization/virtualbox_synaptic_select_tools.png
    :scale: 70 %

Mark "virtualbox-ose-guest-utils" for installation.

  .. image:: /images/projects/virtualization/virtualbox_synaptic_apply.png
    :scale: 70 %

Apply the changes.

Reboot the virtual machine and the display settings should match your host
computer's display settings. These can be changed from the main menu via:

Select: :menuselection:`Preferences --> Monitor Settings` or `ARandR`

See Also:
--------------------------------------------------------------------------------

 * :doc:`osgeolive_quickstart`
 * :doc:`osgeolive_install_quickstart`
 * :doc:`usb_quickstart`

