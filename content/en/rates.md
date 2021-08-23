---
title: Rates
description: "The Official Forex API Developer Guide."
position: 2
category: Guide
---

<alert type="warning">

To get access of those endpoint, you need [API Key](https://forexapi.world/settings/api)

</alert>

## Fetch

Get the latest exchange rates available currencies.

### Example

<code-group>
  <code-block label="cURL" active>

```cURL
curl https://api.forexapi.world/rates
-H "X-API-Key: YOUR_API_KEY"
-X GET
```

  </code-block>
</code-group>

### Result format

```json
[

    {
    "name": "Afghanistan, Afghani",
    "code": "AFN",
    "symbol": "؋",
    "format": "؋1,0.0000",
    "exchange_rate": "77.243354",
    "updated_at": "2021-01-10T15:30:24.000000Z"
  },
  {
    "name": "Albania, Lek",
    "code": "ALL",
    "symbol": "Lek",
    "format": "1,0.00Lek",
    "exchange_rate": "101.235184",
    "updated_at": "2021-01-10T15:30:24.000000Z"
  },
  {
    "name": "Algerian Dinar",
    "code": "DZD",
    "symbol": "د.ج‏",
    "format": "د.ج‏ 1,0.0000",
    "exchange_rate": "132.206578",
    "updated_at": "2021-01-10T15:30:27.000000Z"
  },
  ...
]
```

## Only one currency

Get the latest exchange rates for a currency.

### Example

<code-group>
  <code-block label="cURL" active>

```cURL
curl https://api.forexapi.world/rates?for=AFN
-H "X-API-Key: YOUR_API_KEY"
-X GET
```

  </code-block>
</code-group>

### Result format

```json
{
  "name": "Afghanistan, Afghani",
  "code": "AFN",
  "symbol": "؋",
  "format": "؋1,0.0000",
  "exchange_rate": "77.243354",
  "updated_at": "2021-01-10T15:30:24.000000Z"
}
```

## Only one currency & convert

Get the latest exchange rates for a currency and convert response.

### Example

<code-group>
  <code-block label="cURL" active>

```cURL
curl https://api.forexapi.world/rates?for=USD&base=xaf
-H "X-API-Key: YOUR_API_KEY"
-X GET
```

  </code-block>
</code-group>

### Result format

```json
{
  "name": "US Dollar",
  "code": "USD",
  "symbol": "$",
  "exchange_rate": "560.79",
  "updated_at": "2021-01-10T15:30:24.000000Z"
}
```
