# Vehicle Catalog

**Vehicle brands and models in CSV and JSON.**

[Русская версия](README.ru.md) · [CSV](vehicles.csv) · [JSON](vehicles.json)

Vehicle Catalog is a reference dataset for vehicle pickers, search, and data normalization. It covers passenger cars, trucks, motorcycles, and other types of vehicles. Each row contains a category, a brand, and a model name.

## Dataset at a glance

**5,488 model entries · 554 brand entries · 11 categories**

The files represent the snapshot taken on **30 October 2026**. A brand listed in multiple categories is counted once per category. Original spellings are preserved, including Cyrillic and other non-ASCII characters.

| Category | Brand entries | Model entries |
| --- | ---: | ---: |
| Passenger cars | 397 | 4,541 |
| Trucks | 20 | 138 |
| Motorcycles | 18 | 154 |
| ATVs | 14 | 70 |
| UTVs and buggies | 15 | 77 |
| Snowmobiles | 8 | 44 |
| Personal watercraft | 5 | 29 |
| Boats | 20 | 122 |
| Special equipment | 20 | 129 |
| Trailers | 18 | 88 |
| Other | 19 | 96 |

## Files and format

| File | Contents |
| --- | --- |
| [vehicles.csv](vehicles.csv) | UTF-8 CSV with a header row. |
| [vehicles.json](vehicles.json) | UTF-8 JSON array with the same rows in the same order. |

Each entry has three fields.

| Field | Meaning |
| --- | --- |
| `category` | Vehicle category, such as `passenger_car` or `motorcycle`. |
| `brand` | Brand name as recorded in the catalog. |
| `model` | Model name as recorded under that brand. |

```json
{
  "category": "passenger_car",
  "brand": "Abarth",
  "model": "124 Spider"
}
```

## Sources and verification

According to the maintainer, the catalog entries were collected manually by looking up individual brands and models and checking them against publicly accessible sources. These include manufacturer websites and archives, where available. Source links were retained for some entries.

The export was checked for duplicate names within each category or brand, invalid characters, and mismatches between brand and model categories. Passenger-car names were also compared with external catalogs.

## Reporting a correction

Include the category, brand, and model exactly as listed, the proposed change, and a public source. For regional names or aliases, include the market and explain how the names are related.

## Data license

A license for redistribution and reuse has yet to be selected.
