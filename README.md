# o3csf
Compiles text files into encrypted, non-readable .o3scf format and decompiles them back with a password. In one local browser application.

----------------------------
O3SCF File Encryptor WebApp 
----------------------------

DISCLAIMER
----------
>>> O3SCF COMES WITH ABSOLUTELY NO WARRANTY. <<<
>>> ANY LIABILITY IS EXPRESSLY DISCLAIMED.   <<<
>>> Copyright (c) openw3rk INVENT            <<<
------------------------------------------------------------ 

DESCRIPTION
-----------
O3SCF is an open-source browser-based tool that allows you to
compile and decompile source/text files such as:
- .txt
- .js
- .html
- .c

Files are encrypted into a proprietary format (.o3scf) that is
only readable and reversible using this tool and the correct
password.

No installation or backend required — everything runs in your
browser.

------------------------------------------------------------
FEATURES
--------
- AES-GCM encryption using a password
- Encrypted metadata (original file name and extension)
- Password-protected decompilation
- 10-second lock after 3 incorrect password attempts
- File is restored with original formatting, content and extension
- 100% client-side, open-source, free to use

------------------------------------------------------------
HOW IT WORKS
------------

COMPILING:
- Upload a supported file
- Enter a password
- The file content and metadata are encrypted
- You get a .o3scf file

DECOMPILING:
- Upload a .o3scf file
- Enter the correct password
- The file is decrypted and restored to:
  originalName-originalExtension-decompiled.originalExtension

Example:
  script.js  -->  script.js.o3scf
  Then decompiled: script-js-decompiled.js

------------------------------------------------------------
SUPPORTED FILE FORMATS
-----------------------
.txt
.js
.html
.c

(Other plaintext files may work but are not officially supported.)

------------------------------------------------------------
SECURITY BEHAVIOR
------------------
- After 3 wrong passwords, the app locks decryption for 10 seconds
- Metadata and file content are encrypted with AES-GCM
- Password-derived encryption key using PBKDF2

------------------------------------------------------------
FILE STRUCTURE (.o3scf)
------------------------
1. Salt (random)
2. IV (initialization vector)
3. Encrypted metadata (original name + extension)
4. Encrypted file content

------------------------------------------------------------
DISCLAIMER & WARRANTY
----------------------
O3SCF is open-source and free software.

>>> O3SCF COMES WITH ABSOLUTELY NO WARRANTY. <<<
>>> ANY LIABILITY IS EXPRESSLY DISCLAIMED.   <<< 

Use at your own risk. Do not rely on this software for
sensitive or mission-critical applications.

------------------------------------------------------------
LICENSE
-------
O3SCF is licensed under the MIT License.
You are free to use, modify, and redistribute the software
according to the terms of that license.

