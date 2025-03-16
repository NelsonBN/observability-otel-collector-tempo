# Observability - Otel Collector & Grafana/Tempo

## How can I use it?

After setting up the docker-compose, you need to attach the terminal to the container to control the TUI.
```bash
docker attach otel-tui
```

### Generate signals
```bash
docker attach telemetrygen
telemetrygen traces --traces 1 --otlp-insecure --otlp-endpoint otel-collector:4317
```

## References

### Tempo
- [Quickstart](https://grafana.com/docs/tempo/latest/getting-started/docker-example/)

### OpenTelemetry
- [Exporters](https://github.com/open-telemetry/opentelemetry-collector/tree/main/exporter/otlphttpexporter)

### Grafana
- [MLTP](https://github.com/grafana/intro-to-mltp)
