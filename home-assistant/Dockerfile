FROM homeassistant/home-assistant:stable

COPY . /imported

# Override volume configuration with imported on runtime
CMD cp -a /imported/. /config && python -m homeassistant --config /config