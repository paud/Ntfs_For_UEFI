# Compile
    The project should be compiled under edk2 with edk2-libc project. 
    Copy StdLib, StdLibPrivateInternalFiles and Ntfs_For_UEFI to root of edk2 project
    Comment the following line in LibC.inf of StdLib
    [LibraryClasses]
        #ShellCEntryLib
    
# Description for folders
    The library folder is Ntfs-3g source code modified a little. 
    The NtfsDxe folder is simple file system abstracting the NTFS. 
    The Conf folder is sample for building configuration of edk2.
    The bin folder is bin file prebuilding

# User guild
        Run following command under uefi shell, the NTFS volume will be mounted and can be explored.
        >>load NftsDxe.efi
        >>map
        
# Limitation
        1. Don't support the volume with bit locker
        ...
