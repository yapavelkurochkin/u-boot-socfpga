There can be a problem with 'openssl' build dependencies. This repo requires 1.0.0, but on your build system it can be newer...

To overcome it, please clone git@github.com:openssl/openssl.git (branch OpenSSL_1_0_0-stable) into openssl/ directory, configure it and build for Host machine:

    ./config
    make -j8

After that, build U-boot & SPL normally.
