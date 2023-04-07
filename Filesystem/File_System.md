# Linux File System Explained

## bin:
Short for "binaries," the bin folder holds the most basic binary files, such as 'ls' for listing a directory, 'cat' for displaying the contents of a file, and other basic functions are stored here.

## sbin:
The sbin folder contains system binaries that a system administrator would use. Standard users wouldn't have access to these files without proper permissions.

## dev:
The dev folder is where device files live, including those for webcams, keyboards, mice, disks, CPUs, and GPUs. This is where drivers reside, and users should not tamper with this directory.

## etc:
This folder contains configuration files for your system. You can find repositories you're connected to and various settings here. All system-wide configuration files are located in the etc folder.

## lib/lib32/lib64:
These folders house libraries, which are files that applications can use to perform various functions. These libraries are required by the binaries in the 'bin' and 'sbin' folders.

## media/mnt:
These folders are where you'll find other mounted drives, such as USB sticks or external hard drives. The 'media' directory manages external drives automatically through the operating system, while 'mnt' is used for manual management. Most devices will be managed by 'media' automatically.

## opt:
The opt folder is where optional functionality and external software can be found or placed, such as Ledger Live, VPN, Grammarly, etc.

## proc:
The proc folder contains sudo files with information about system processes and resources. For example, every process will have a directory here containing various details about that process.

## root:
Root is the root user's home folder. Unlike the regular 'home' folder, it does not contain directories inside. Folders and files can be placed inside, but root permission is required to access them.

## run:
The run folder contains everything that operates in RAM, which means its contents will be lost upon a system reboot or shutdown.

## snap:

## srv:
The srv folder is the service directory where service data is stored. It will likely be empty, but if you run a server, all data will be stored here for external users to access, allowing for improved security.

## sys:
The sys folder is a way to interact with the kernel. This directory is similar to the 'run' directory and is not physically written to the disk. It is created every time the system boots up, so you should not store anything here and nothing gets installed in this directory.

## tmp:
The tmp folder is a temporary directory where applications like VS Code store temporary copies of files to recover in case of a crash. This folder is usually emptied upon rebooting or shutting down the system.

## usr:
The usr folder is the user applications space, where non-essential applications used by the user will be installed. All essential applications are stored in the 'bin' folder.

## var:
The var folder contains files and directories that are expected to grow in size. For example, 'var/crash' holds information on processes that have crashed, and 'var/log' contains log files.

## home:
In the home folder, each user has their own folder and can only access their own files, unless granted permissions. You can mount this folder on a different drive and restore files and data after reinstalling the OS.
