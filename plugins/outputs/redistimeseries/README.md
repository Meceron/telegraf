# RedisTimeSeries Producer Output Plugin

The RedisTimeSeries output plugin writes metrics to the RedisTimeSeries server.

## Global configuration options <!-- @/docs/includes/plugin_config.md -->

In addition to the plugin-specific configuration settings, plugins support
additional global and plugin configuration settings. These settings are used to
modify metrics, tags, and field or create aliases and configure ordering, etc.
See the [CONFIGURATION.md][CONFIGURATION.md] for more details.

[CONFIGURATION.md]: ../../../docs/CONFIGURATION.md

## Configuration

```toml
[[outputs.redistimeseries]]
  ## The address of the RedisTimeSeries server.
  address = "127.0.0.1:6379"
  ## password to login Redis
  password = ""

  ## username (optional)
  # username = ""
  # redis database number (optional, must be an integer)
  # database = 0

  ## optional TLS configurations
  # tls_ca = "/etc/telegraf/ca.pem"
  # tls_cert = "/etc/telegraf/cert.pem"
  # tls_key = "/etc/telegraf/key.pem"
  # insecure_skip_verify = false
```
