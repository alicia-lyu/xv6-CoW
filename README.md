# Copy-on-Write (CoW) `fork()` in xv6 kernel

This group project implemented with **C** code the Copy-on-Write (CoW) `fork()` in the xv6 kernel. Compared with the original `fork()` which copies all of the parent process's user-space memory into the child, the new implementation only copies the page which the child process tries to write into, increasing memory efficiency.