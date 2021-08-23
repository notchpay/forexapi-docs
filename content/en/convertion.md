---
title: Convertion
description: "The Official Forex API Developer Guide."
position: 4
category: Guide
---

<alert type="warning">

To get access of those endpoint, you need [API Key](https://forexapi.world/settings/api)

</alert>

# Convert

Convert any money value from one currency to another at the latest API rates.

## Formatted result

<code-group>
  <code-block label="cURL" active>

```cURL
curl https://api.forexapi.world/convert?from=USD&to=XAF&value=500
-H "X-API-Key: YOUR_API_KEY"
-H "Content-Type: application/json"
-X GET
```

  </code-block>
</code-group>

Result format

```json
{
  "result": "270,648.40 F.CFA",
  "from": "USD",
  "to": "XAF"
}
```

## Unformatted result

<code-group>
  <code-block label="cURL" active>

```cURL
curl https://api.forexapi.world/convert?from=USD&to=XAF&value=500&format=false
-H "X-API-Key: YOUR_API_KEY"
-H "Content-Type: application/json"
-X GET
```

  </code-block>
</code-group>

Result format

```json
{
  "result": 270648.3995,
  "from": "USD",
  "to": "XAF"
}
```

## Conversion based on country code

<code-group>
  <code-block label="cURL" active>

```cURL
curl https://api.forexapi.world/convert?from=USD&country=cm&value=500
-H "X-API-Key: YOUR_API_KEY"
-H "Content-Type: application/json"
-X GET
```

  </code-block>
</code-group>

Result format

```json
{
  "result": 270648.3995,
  "from": "USD",
  "to": "XAF"
}
```
