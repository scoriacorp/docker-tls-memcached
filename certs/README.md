# TLS certificates for Memcached + TLS testing

Certificate generation is inspired by [badssl.com](https://github.com/chromium/badssl.com)

The certificates need to be renewed once every two years.

The certificates hierarchy is:

  - client-ca-root
    - client

  - ca-root
    - ca-intermediate
      - server-rsa2048
