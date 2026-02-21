## Common Queries 

```kql
PassiveDns

| where url contains "https://..xyz.com"

| where domain contains "xyz.com"
| distinct ip // gets ip address related to domain 

| where ip contains "123"
```

```kql
AuthenticationEvents 

| where username == "xyz"
```

```kql
InboundNetworkEvents //any requests coming into network

| where src_ip == "x.x.x.x"

| where user_agent == "Mozilla 5.0...xyz"
```

```kql
OutboundNetworkEvents // any requests going outside of network (e.g, websites an employee visits)

| where src_ip == "10.10.0.22"

```

```kql
Email
| where sender =~ "afomiya_storm@clouthaus.com"
| where recipient !endswith "@clouthaus.com"
| summarize count() by recipient
| order by count_ desc // this gets how many times the recipient receives emails
```

```kql
Employees
| take 10 // this returns 10 random tables in the Employees table

| count //counts employees or rows in table

| where role == "xyz" //returns specific employee

| where role contains "xyz" //if you only specific word like instead of "security analyst", you could write "security" and find that role

```