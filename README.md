# Std thread loki logs sender for tracing

```rust
let loki_layer = LokiLayer::new(loki_server_url, Default::default());
let subscriber = tracing_subscriber::Registry::default().with(loki_layer);
let quard = tracing::subscriber::set_default(subscriber);
```
