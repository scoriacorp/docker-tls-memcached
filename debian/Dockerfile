FROM memcached:1.6.3

LABEL description="This image is built for TLS testing purposes."

COPY ./certs/gen /opt/certs

CMD [ \
    "memcached", \
    "-Z", \
    "-o", "ssl_verify_mode=1", \
    "-o", "ssl_chain_cert=/opt/certs/chain/server-rsa2048.pem", \
    "-o", "ssl_key=/opt/certs/key/server-rsa2048.key", \
    "-o", "ssl_ca_cert=/opt/certs/crt/client-ca-root.crt" \
]
