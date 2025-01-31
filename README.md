This is an archive of the Rc/Funge Befunge-98 interpreter, since the original site went offline recently. 
rcfunge98.com now points to a malicious website. The original is still on the Wayback Machine on archive.org, but I worry about the malicious site becoming the latest archive, which
could be problematic.

# Files
- `rcfunge.tgz` is the source for Rc/Funge-98 V1
- `rcfunge2.tgz` is the source for Rc/Funge-98 V2. This is probably the one you want
- `funge` (no extension) is a precompiled linux binary for Rc/Funge-98 V2 since it looks like Rc/Funge is abandonware at this point.
  - It is for amd64/x64 Linux, and runs fine on WSL2 (Windows Subsystem for Linux) or on a virtual machine
  - You can either put it in a standard binary folder (like `/usr/bin`, `/usr/local/bin`, etc.), or just run it from the current folder
  - In the latter case, you can call it by `./funge` if it is in the current folder, `../funge` if it is in the parent folder, or by full path otherwise. (Just trying to be as friendly as possible to beginners)
- If you want to compile from source, you'll have to extract the .tgz archive. 7-Zip works with Windows and WSL, otherwise I don't know what program to use because I'm a bit inexperienced with Linux.
- `rcfunge-windows.exe` is a pre-compiled Windows executable built on MinGW. If I did everything right it shouldn't need MinGW to run; I plan to send it to my other computer to test that out. It's for x86_64,
  which is the most common but there are also ARM-based Windows devices and 32-bit devices which this will not run on.
  - There are some limitations in this version, specifically that the FORK, NCRS, SGNE, SGNL, SOCK, SCKE, TERM, WIND, TURT, REXP (due to some glitchy MinGW compiler behavior), MSGQ, SMEM, SMPH, and UNIX fingerprints are
    missing. Most of the rest is not tested but is compiled into the executable and will hopefully work.
- `rcfunge-windows.patch` is the patch applied to the rcfunge source tree to make it work.
