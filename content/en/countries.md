---
title: Countries
description: "The Official Forex API Developer Guide."
position: 5
category: Guide
---

<alert type="warning">

To get access of those endpoint, you need [API Key](https://forexapi.world/settings/api)

</alert>

# Fetch

Get countries list available on our server.

<code-group>
  <code-block label="cURL" active>

```cURL
curl https://api.forexapi.world/countries
-H "X-API-Key: YOUR_API_KEY"
-H "Content-Type: application/json"
-X GET
```

  </code-block>
  
</code-group>

Result format

```json
[
  {
"name": "Afghanistan",
"iso2": "AF"
},
{
"name": "Åland Islands",
"iso2": "AX"
},
{
"name": "Albania",
"iso2": "AL"
},
{
"name": "Algeria",
"iso2": "DZ"
},
{
"name": "American Samoa",
"iso2": "AS"
},
{
"name": "Andorra",
"iso2": "AD"
},
{
"name": "Angola",
"iso2": "AO"
},
{
"name": "Anguilla",
"iso2": "AI"
}
  ...
]
```
