FROM homeassistant/home-assistant:stable

COPY . /imported

# Install HACS
RUN wget -q -O - https://install.hacs.xyz | bash -

# Override volume configuration with imported on runtime
CMD cp -a /imported/. /config && python -m homeassistant --config /config