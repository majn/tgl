# Telegram library

This is library that handles Telegram API and protocol.

> This is a fork of [vysheng's repository](https://github.com/vysheng/tgl).

This variant focuses mostly on the use for the [purple plugin](https://github.com/majn/telegram-purple).

If you're looking for client CLI implementation, check [TG repository](https://github.com/vysheng/tg) instead. 

Build status:

| Repository                                             | Status|
| ------------------------------------------------------ | ----- |
| [vysheng](https://github.com/vysheng/tgl) (main)       | [![Build Status](https://travis-ci.org/vysheng/tgl.svg)](https://travis-ci.org/vysheng/tgl) |
| [kenorb-contrib](https://github.com/kenorb-contrib/tgl) | [![Build Status](https://travis-ci.org/kenorb-contrib/tgl.svg)](https://travis-ci.org/kenorb-contrib/tgl) |
| [majn](https://github.com/majn/tgl) | [![Build Status](https://travis-ci.org/majn/tgl.svg)](https://travis-ci.org/majn/tgl) |

Current versions:

- `scheme.tl`: Layer 38
- `encrypted_scheme.tl`: Layer 23

### API, Protocol documentation

Documentation for Telegram API is available here: https://core.telegram.org/api

Documentation for MTproto protocol is available here: https://core.telegram.org/mtproto

### Installation

Clone this GitHub repository with `--recursive` parameter to clone submodules.

     git clone --recursive https://github.com/majn/tgl.git && cd tgl

#### Linux and BSDs

Install libs: openssl, zlib
if you want to use provided net/timers then install libevent and add --enable-libevent key to configure

You can also avoid the OpenSSL dependency: Install gcrypt (>= 1.60, Debian derivates know it as "libgcrypt20-dev"), and add --disable-openssl key to configure

Then,

     ./configure
     make
