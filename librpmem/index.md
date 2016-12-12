---
title: librpmem
layout: nvml
---

#### The librpmem library

**librpmem** provides low-level support for remote access to
*persistent memory* (pmem) utilizing RDMA-capable RNICs. The library can be
used to replicate remotely a memory region over RDMA protocol.
It utilizes appropriate persistency mechanism based on remote node's platform
capabilities. The **librpmem** utilizes the **ssh** client to authenticate
a user on remote node and for encryption of connection's out-of-band
configuration data. See **SSH** section for details.

This library is for applications that use remote persistent memory directly,
without the help of any library-supplied transactions or memory
allocation. Higher-level libraries that build on **libpmem** are
available and are recommended for most applications, see:

Man pages that contains a list of the interfaces provided:

* Man page for [librpmem current master](../manpages/master/librpmem.3.html)
* Latest releases:
   * Man page for [librpmem version 1.2](../manpages/v1.2/librpmem.3.html)

#### The rpmemd utility

The **rpmemd** process is executed on target node by **librpmem** library over
**ssh**(1) and facilitates access to persistent memory over RDMA.

See the [rpmemd man page](../manpages/master/rpmemd.1.html)
for current master documentation and examples.

#### librpmem Examples

**More Detail Coming Soon**

<code data-gist-id='krzycz/f8c6827b536fc42399db58cf30007e96' data-gist-file='manpage.c' data-gist-line='36-81' data-gist-highlight-line='39' data-gist-hide-footer='true'></code>
