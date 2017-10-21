FROM schecbr/todobackend-base:latest
MAINTAINER Brian Scheck <schecbr@gmail.com>

# Copy application artifacts
COPY target /wheelhouse

# Install application
RUN . /appenv/bin/activate && \
    pip install --no-index -f /wheelhouse todobackend && \
    rm -rf /wheelhouse