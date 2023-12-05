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
