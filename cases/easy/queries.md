## Common Queries 

```kql
PassiveDns

| where url contains "https://..xyz.com"
| where domain contains "xyz.com"
| where ip contains "123"
```

```kql
AuthenticationEvents 

| where username == "xyz"
```

```kql
InboundNetworkEvents

| where src_ip == "x.x.x.x"
| where user_agent == "Mozilla 5.0...xyz"
```
