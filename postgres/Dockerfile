FROM postgres

COPY  run.sh /
CMD [ "/run.sh" ]

# Labels
LABEL \
    io.hass.name="Postgres" \
    io.hass.description="A PostgreSQL database server" \
    io.hass.arch="${BUILD_ARCH}" \
    io.hass.type="addon" \
    io.hass.version=${BUILD_VERSION} \
    maintainer="Westenberg" \
    org.opencontainers.image.title="Postgres" \
    org.opencontainers.image.description="A PostgreSQL database server" \
    org.opencontainers.image.vendor="Home Assistant Community Add-ons" \
    org.opencontainers.image.authors="Westenberg" \
    org.opencontainers.image.licenses="MIT" \
    org.opencontainers.image.url="https://addons.community" \
    org.opencontainers.image.source="https://github.com/westenberg/hassio/blob/master/postgres" \
    org.opencontainers.image.documentation="https://github.com/westenberg/hassio/blob/master/postgres/README.md" \
    org.opencontainers.image.created=${BUILD_DATE} \
    org.opencontainers.image.revision=${BUILD_REF} \
    org.opencontainers.image.version=${BUILD_VERSION}
