FROM xirixiz/dsmr-reader-docker

RUN apk add sed
COPY entrypoint.sh /
RUN echo "X_FRAME_OPTIONS = 'ALLOWALL'" >> dsmrreader/settings.py
ENTRYPOINT /entrypoint.sh

# Labels
LABEL \
    io.hass.name="DSMR-reader" \
    io.hass.description="Extract and store data transferred by the DSMR protocol of your smart meter." \
    io.hass.arch="${BUILD_ARCH}" \
    io.hass.type="addon" \
    io.hass.version=${BUILD_VERSION} \
    maintainer="Westenberg" \
    org.label-schema.description="Extract and store data transferred by the DSMR protocol of your smart meter." \
    org.label-schema.build-date=${BUILD_DATE} \
    org.label-schema.name="DSMR-reader" \
    org.label-schema.schema-version="1.0" \
    org.label-schema.url="https://addons.community" \
    org.label-schema.usage="https://github.com/westenberg/hassio/blob/master/dsmr-reader/README.md" \
    org.label-schema.vcs-ref=${BUILD_REF} \
    org.label-schema.vcs-url="https://github.com/westenberg/hassio" \
    org.label-schema.vendor="Community Hass.io Addons"
