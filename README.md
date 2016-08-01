# vcdliveimport

This script is a PowerShell .PS1 file to allow administrators to live-import running VMs from a vSphere environment into VMware vCloud Director.

The script needs to be executed from an environment where it can connect to both the vCloud Director API and the vCenter host in order to function.

The credentials entered need to be administrative/system level for both vCloud Director AND vCenter.

The minimum vCloud Director level supported is v8.10 as the API function for live import was only added in this version.

Change the destination vCloud API endpoint in line 2 to match the URL for your vCloud Director instance.

The imported VM will be placed in a vApp named the same as the VM in the Virtual Datacenter (VDC) selected when the script is run.
