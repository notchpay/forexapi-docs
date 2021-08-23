---
title: Currencies
description: "The Official Forex API Developer Guide."
position: 3
category: Guide
---

<alert type="warning">

To get access of those endpoint, you need [API Key](https://forexapi.world/settings/api)

</alert>

# Fetch

Get currencies available on our server.

### Example
<code-group>
  <code-block label="cURL" active>

```cURL
curl https://api.forexapi.world/currencies
-H "X-API-Key: YOUR_API_KEY"
-H "Content-Type: application/json"
-X GET
```

  </code-block>
  
</code-group>

### Result format

```json
[
  {
    "mame": "Afghan Afghani",
    "code": "AFN"
  },
  {
    "mame": "Albanian Lek",
    "code": "ALL"
  },
  {
    "mame": "Algerian Dinar",
    "code": "DZD"
  },
  {
    "mame": "Angolan Kwanza",
    "code": "AOA"
  },
  ...
]
```
