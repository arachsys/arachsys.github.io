# Chris Webb

This is Chris Webb's home page. The best way to contact me is by email to
[chris@arachsys.com](mailto:chris@arachsys.com). You can also follow me as
[@arachsys](https://bsky.app/profile/arachsys.bsky.social) on Bluesky,
as [@dairychris](https://twitter.com/dairychris) on Twitter, or [find me
on Facebook](https://facebook.com/arachsys), although I'm not very active
on social media nowadays.


## Farming life

I'm a beef farmer and calf rearer in North Shropshire. I tweet photographs,
occasional rants about agricultural technology, and general updates on the
cattle and my day-to-day farming exploits as
[@dairychris](https://twitter.com/dairychris) on Twitter.


## Free software

A number of my free software projects are available on
[GitHub](https://github.com/arachsys),
[BitBucket](https://bitbucket.org/arachsys),
[Codeberg](https://codeberg.org/arachsys),
[GitLab](https://gitlab.com/arachsys) and
[Sourcehut](https://git.sr.ht/~arachsys). You might be looking
for:

- [containers](https://github.com/arachsys/containers) --- lightweight
  containers using Linux namespaces

  This package is a minimalist implementation of containers for Linux,
  making secure containers as easy to create and use as a traditional
  chroot. It comprises three utilities, contain, inject and pseudo, which
  use the kernel support for user namespaces merged in Linux 3.8. See also
  [ucontain](https://github.com/arachsys/ucontain), a simplified shell
  script reimplementation.

- [cts-tool](https://github.com/arachsys/cts-tool) --- a command-line
  interface to the British cattle tracing system

  The British Cattle Movement Service run a tracing database for farmers to
  record cattle births, deaths and movements. This command-line interface
  to their XML-over-HTTP API is an alternative to the clunky web frontend.

- [init](https://github.com/arachsys/init) --- a BSD-style init, daemon,
  syslog and udev replacement

  A lightweight init suite used in Arachsys Linux, this is a toolkit of
  small utilities including a daemon wrapper supporting asynchronous
  dependencies and listening sockets, a simple but flexible syslog
  implementation, an elegant replacement for the increasingly bloated udev
  daemon, and a template `/etc/init` written as a simple shell script.

- [libelf](https://github.com/arachsys/libelf) --- freestanding libelf
  extracted from elfutils

  This builds cleanly without autotools on both musl and glibc, using either
  clang or gcc. On musl systems it doesn't need extra argp, fts or obstack
  libraries, just zlib for handling compressed ELF sections.

- [mailflow](https://github.com/arachsys/mailflow) and
  [mailwrap](https://github.com/arachsys/mailwrap) --- improved plain text
  email in Apple Mail

  I sometimes work on an Apple machine running macOS, and it used to be
  convenient to use the built-in IMAP mail client. It wasn't too bad for
  reading mail, but whilst it once emitted nice RFC2646 *format=flowed*
  message bodies, recent releases horribly mangle plain text with a
  quoted-printable transfer encoding.

  MailFlow monkey-patched Apple Mail to emit *format=flowed* plain text
  messages, also fixing problems with displaying leading whitespace, and
  quoting/attribution in replies. MailWrap is an earlier plugin to add
  a manual line-wrapping and paragraph filling shortcuts in the message
  composer. Unfortunately, plugins like these are no longer possible on
  the most recent releases of Apple Mail, though the bugs and problems
  they worked around are still glaringly obvious.

- [microdns](https://github.com/arachsys/microdns) --- authoritative name
  server based on Dan Bernstein's tinydns

  This is my fork of Dan's public domain tinydns, reworked and updated for
  modern RFC compliance, efficient multiplexed TCP service and full IPv6
  support. It is actively maintained but has diverged a bit from the
  classic codebase.

- [montage](https://arachsys.github.io/montage/) --- resources for Yamaha
  Montage synthesisers

  These include simple utilities, reverse-engineered file formats,
  undocumented sysex commands, instructions for obtaining a shell, and
  hardware notes.

- [neova](https://github.com/arachsys/neova) --- a tool to configure the
  Enhancia Neova ring controller

  This command-line interface covers the same functions as the graphical
  Neova Dashboard application but is portable, scriptable and more
  convenient to use.

- [nobmc](https://arachsys.github.io/nobmc/) --- hardware to reset and
  power-cycle servers using serial console breaks

  These small boards were designed to allow remote management of Arachsys
  servers over an RS232 serial console, bypassing the integrated BMCs which
  are clunky, unreliable and horribly insecure.

- [openntpd](https://github.com/arachsys/openntpd) --- alternative
  multiplatform openntpd

  This is an alternative multiplatform repackaging of OpenBSD's openntpd,
  compatible with Linux glibc, Linux musl, FreeBSD, NetBSD and DragonFly,
  as well as the original OpenBSD. It is actively maintained, includes a
  number of fixes and quality-of-life improvements and isn't obfuscated
  by autoconf, automake and libtool.

- [pocketcrypt](https://github.com/arachsys/pocketcrypt) --- a lightweight
  legacy-free cryptographic library

  Pocketcrypt is a tiny legacy-free cryptographic library providing duplex
  constructions using NIST LWC finalists Gimli and Xoodoo, together with
  standard X25519 for key exchange and Schnorr signatures. Eschewing
  interoperability with the standard museum of primitives and protocols, it
  offers concise, easily-understood and easy-to-audit code that avoids the
  ugly boilerplate and obfuscation of larger libraries.

- [ptywrap](https://github.com/arachsys/ptywrap) --- wrap stdout and/or
  stderr with a pseudoterminal

  Some programs (such as compilers and build systems) colour their output
  only when it is directed to a terminal. This wrapper provides an easy
  way to trigger this behaviour when logging to a file or pipe instead.

- [qoget](https://github.com/arachsys/qoget) -- Qobuz download tool

  This is a command-line client to the Qobuz music streaming service.
  Tracks are retrieved in FLAC format and are automatically tagged with
  Vorbis comments based on the Qobuz metadata. There are no dependencies
  other than the Python standard library.

- [skd](https://github.com/arachsys/skd) --- attach scripts to unix, IPv4 or
  IPv6 listening sockets

  skd is my original socket daemon, written as an inetd replacement in the
  mid-1990s. It binds to a UDP, TCP or unix socket, waits for connections
  and runs a specified program to handle them. See also the daemon utility
  in my more recent [init](https://github.com/arachsys/init) suite which
  can listen on TCP and unix sockets in a similar way and is a better choice
  for new applications.

- [ssh-x25519](https://github.com/arachsys/ssh-x25519) --- map
  ssh-ed25519 keys into x25519 keys

  This trivial wrapper around standard Go crypto libraries converts OpenSSH
  ssh-ed25519 identities to x25519 keys for use in other contexts such as
  file encryption or key exchange, compatible with simple, easy-to-audit
  x25519 libraries like Pocketcrypt.

- [tinyacme](https://github.com/arachsys/tinyacme) --- order certificates
  using ACME TLS-ALPN-01

  These small stand-alone utilities automatically provision/renew TLS
  certificates from ACME-based providers such as Let's Encrypt.

- [tinymbim](https://github.com/arachsys/tinymbim) --- bring up a mobile
  internet connection using MBIM

  Tinymbim is a command-line utility to control an MBIM-compatible mobile
  broadband modem on Linux using its cdc-wdm control device.

- [tinyquota](https://github.com/arachsys/tinyquota) --- control filesystem
  quotas on Linux

  These tools manipulate block and file quotas by user, group or project ID,
  taking advantage of the native quota support in ext4 and xfs.

- [tube](https://github.com/arachsys/tube) --- an authenticated bidirectional
  peer-to-peer pipe using Pocketcrypt

  This is a worked example which generalises Magic Wormhole's style of
  peer-to-peer file transfer into a bidirectional pipe. Peers authenticate
  with a short shared secret and a PAKE. Both rendezvous server and client
  are fully implemented but at present they are only documented in the
  [design discussion](https://github.com/arachsys/tube/commit/783826c8281b97da3cdfa21093d358e596d73874)
  in the git commit log. The client, server and cryptographic library span
  fewer than 1100 lines of C in total.

- [typetofocus](https://github.com/arachsys/typetofocus) --- streamlined
  window focus for macOS

  As an occasional user of macOS, I'm often frustrated by the clumsy
  click-to-focus model. Traditional point-to-focus doesn't work well with
  the global menu bar, but TypeToFocus implements an interesting variant
  which cooperates well with the rest of the interface.

- [ucom](https://github.com/arachsys/ucom) --- a cruft-free serial terminal

  ucom is a serial terminal in the style of cu, minicom and GNU screen,
  but without legacy modem control, file transfer or a nested terminal
  emulation layer. In fewer than 150 lines of C, it provides a clean
  interactive session with a serial port, aiming for both correctness
  and efficiency.

- [ucontain](https://github.com/arachsys/ucontain) --- a simplified bash
  version of containers using unshare and pivot

  This demonstrates how to use namespaces and ad hoc containers in scripts,
  wrapping unshare and nsenter from util-linux, newuidmap and newgidmap
  from shadow-utils, pivot and seal from Arachsys init. See also the
  original [containers](https://github.com/arachsys/containers) package.

- [webmidi](https://arachsys.github.io/webmidi/) --- a series of
  self-contained Web MIDI tools

  Each single-page application interacts with attached MIDI instruments
  using the Web MIDI API, runs entirely client-side and depends on no
  resources outside its static HTML file.

- [zf](https://github.com/arachsys/zf) --- a compressor-based spam filter

  This abuses zstd dictionary compression to classify inbound email.
  The technique is straightforward and inexpensive but nonetheless
  achieves state-of-the-art filtering accuracy with realistic training
  sets of a few thousand messages per category. See also my earlier
  [af](https://github.com/arachsys/af) filter which wrapped the OSBF-Lua
  module to achieve similar filtering performance.

Other bits and pieces including personal scripts, Yamaha synthesiser
stuff and Arachsys Linux package trees can be found amongst my [public
repositories](https://github.com/arachsys).

Please [contact me by email](mailto:chris@arachsys.com) with any comments,
bug reports or proposed patches, rather than using GitHub web-based pull
requests or issues.


## Linux distribution

Since late 1999, I've maintained Arachsys Linux, an opinionated 'from
scratch' Linux distribution for my development machines and production
servers, porting from 32-bit x86 to x86-64 and arm64 in the mid-2000s. More
recently, I've also deployed it on arm32 routers and arm64 embedded
projects.

Unusual features include [musl libc](https://musl.libc.org/), support for
both llvm and gcc toolchains, a simple shell-script `/etc/init` assisted by
my [init tools](https://github.com/arachsys/init), and a willingness to
clean up cruft at the expense of legacy compatibility. There is no `/usr`,
`/sbin`, `/include` or `/share` on an Arachsys Linux system, just `/bin`
and `/lib`. Shared and static libraries live in `/lib/shared` and
`/lib/static` respectively, with headers in `/lib/include`.

Consumer distributions invariably stuff `/etc` with hundreds of default
config files filled with comments that should be documentation, whereas an
Arachsys `/etc` only contains a handful of files deliberately written by
the user. Similarly, the distribution embraces the trend to tidy
user-specific configuration into `~/.config`, patching programs to enforce
this where necessary. For example, bash, readline and ssh are configured
from `~/.config` although none of these are likely to support this
upstream.

Software is packaged properly so `pkg-config` and friends are redundant.
Libraries are on the standard link path if they are available; header files
are on the standard include path if they are available. As a result, the
filesystem isn't littered with `.la` and `.pc` droppings.

Build recipes now include upstream URLs so the `pkg` tool can check for new
releases across the entire tree. This eliminates the need to track updates
manually, which is time-consuming and error-prone with large numbers of
packages.

My limited time as a solo maintainer means there is little documentation
other than the [package tree](https://github.com/arachsys/packages) and
[commit log](https://github.com/arachsys/packages/commits), but the `pkg`
build tool is written in clear, easy-to-read bash and is maintained
[in tree](https://github.com/arachsys/packages/tree/master/pkg). I upload
periodic snapshots of the binary images needed to bootstrap a system on
the [GitHub releases](https://github.com/arachsys/packages/releases) page.


## Curve25519 public key

My long-term public identity is the elliptic curve point represented in
OpenSSH format as `ssh-ed25519
AAAAC3NzaC1lZDI1NTE5AAAAIMHPkQPn4+cxxP2Ax29Ozhkvu7Vp0KMlPAncD6fFmqCb` and in
base64-encoded X25519 form as
`cyUynIqlEg8JL96nxStP4LKfECrYomQXrAdC6jurVwE=`.

I use the corresponding private key to sign releases and git tags, and to
authenticate myself more generally.
