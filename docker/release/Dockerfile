FROM jkoskiaho/todobackend-base:latest
MAINTAINER Juha Koskiaho <dev.jkoskiaho@outlook.com>

# Copy application artifacts
COPY target /wheelhouse

# Install application
RUN . /appenv/bin/activate && \
    pip install --no-index -f /wheelhouse todobackend && \
    rm -fr /wheelhouse
