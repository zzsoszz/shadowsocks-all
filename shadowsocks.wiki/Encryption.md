Supported Ciphers
=================

                   |  Python   |    libev    |     Go    |     Qt
------------------ | --------- | ----------- | ----------| ---------
SSL library (AES, etc) |     Y     |      Y      |      Y    |     Y
RC4-MD5            |     Y     |      Y      |      Y    |     Y
Salsa20, Chacha20  |     Y     |      Y      |      Y    |     Y

For supported ciphers, please refer to [Cipher](https://shadowsocks.org/en/spec/cipher.html) page in shadowsocks.org.

Installing `M2Crypto` will make encryption a little faster.

Debian:

    apt-get install python-m2crypto

CentOS:

    yum install m2crypto

rc4-md5
=======
`rc4-md5` is a safe, fast encryption that use different key per connection. It is recommended for OpenWRT routers.

salsa20 and chacha20
====================
`salsa20` and `chacha20` are fast stream ciphers. Optimized `salsa20` implementation on x86_64 is even 2x faster than `rc4` (but slightly slower on ARM).

Install [libsodium](https://github.com/jedisct1/libsodium) >= 1.0.0 if you want to use them.

    sudo apt-get install build-essential
    wget https://github.com/jedisct1/libsodium/releases/download/1.0.8/libsodium-1.0.8.tar.gz
    tar xf libsodium-1.0.8.tar.gz && cd libsodium-1.0.8
    ./configure && make -j2
    sudo make install
    sudo ldconfig

Deprecated Ciphers
==================
These legacy ciphers are either slow or not safe. Do not use them:
- rc4
- des-cfb
- table
- salsa20-ctr
