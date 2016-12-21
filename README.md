# PoshKPBrute

Powershell Keepass 2.34 Brute Force Tool - crack-keepassfile

.SYNOPSIS
  
  This script provides a simple dictionary based brute force function called crack-keepassfile that allows you to run a dictionary file against a KeePass 2.34 .kdbx file.  
  If it finds the key, it will dump all passwords as output as well as inform you of the master password.

.DESCRIPTION
  
  The script performs a dictionary attack against keepass .kdbx files

.PARAMETER binpath
    
    This is the path for the KeePass 2.34 files - Typically on a default install will be "c:\program files (x86)\KeePass2x\"


.PARAMETER pwdpath
    
    This is the path for the password file to use in the brute force attempt

.PARAMETER targetfile
    
    This is the path for the target kdbx file

.NOTES
  Version:        0.1
  Author:         Wayne Evans
  Creation Date:  20/12/2016
  Purpose/Change: Initial script development

  This script is quite slow, but will get the job done - It works at about 500 keys per second currently.  
  
.EXAMPLE

crack-keepassfile -binpath "C:\program files (x86)\KeePass2x" -pwdfile "c:\software\pwdlist.txt" -targetfile "c:\software\posh.kdbx"

.TODO

1)allow generated patterns to be used to brute force rather than a dictionary file

  
#>
