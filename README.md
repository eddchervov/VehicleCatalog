# Vehicle Catalog

**Vehicle brands and models in CSV and JSON.**

[Русская версия](README.ru.md) · [CSV](vehicles.csv) · [JSON](vehicles.json)

Vehicle Catalog is a reference dataset for vehicle pickers, search, and data normalization. It covers passenger cars, trucks, motorcycles, and other types of vehicles. Each row contains a category, a brand, and a model name.

## Dataset at a glance

**5,549 model entries · 560 brand entries · 11 categories**

Last updated **23 November 2026**. A brand listed in multiple categories is counted once per category. Original spellings are preserved, including Cyrillic and other non-ASCII characters.

| Category | Brand entries | Model entries |
| --- | ---: | ---: |
| Passenger cars | 401 | 4,594 |
| Trucks | 22 | 141 |
| Motorcycles | 18 | 159 |
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

## Update history

### 23 November 2026

Added **61 models** across three categories and introduced five brands: **FUSO, LEPAS, Microlino, Shangjie, Togg**. Tesla also gained a truck entry.

<details>
<summary>All 61 added models</summary>

| Category | Brand | Added models |
| --- | --- | --- |
| Passenger cars | Audi | E5 Sportback |
| Passenger cars | Changan | Deepal L06 |
| Passenger cars | Chevrolet | Equinox EV, Silverado EV |
| Passenger cars | Cupra | Raval |
| Passenger cars | GAC Aion | i60 |
| Passenger cars | Hyundai | IONIQ 3 |
| Passenger cars | Kia | EV2 |
| Passenger cars | Leapmotor | A05, A10 (B03X), B05 (Lafa5), D99 |
| Passenger cars | LEPAS | L4, L6, L8 |
| Passenger cars | Mahindra | BE 6, XEV 9e, XEV 9S, XUV 3XO |
| Passenger cars | Microlino | Microlino |
| Passenger cars | Nio | ES9, Onvo L80, Onvo L90 |
| Passenger cars | Perodua | Aruz, Ativa, Axia, Bezza, QV-E, Traz |
| Passenger cars | Polestar | 5 |
| Passenger cars | Proton | e.MAS 5, e.MAS 7, S70, X90 |
| Passenger cars | Rivian | R2 |
| Passenger cars | Shangjie | H5, Z7, Z7T |
| Passenger cars | Skoda | Epiq |
| Passenger cars | Tata | Altroz, Harrier, Punch, Tiago |
| Passenger cars | Tesla | Cybercab |
| Passenger cars | Togg | T10F, T10X |
| Passenger cars | VinFast | Limo Green, VF 2, VF 3, VF 5 |
| Passenger cars | Xpeng | G9L, L03 |
| Passenger cars | Zeekr | 7GT (007 GT) |
| Trucks | FUSO | eCanter |
| Trucks | Mercedes-Benz | eActros 600 |
| Trucks | Tesla | Semi |
| Motorcycles | Honda | CB1000 Hornet, NT1100, XL750 Transalp |
| Motorcycles | Yamaha | Tracer 7, XSR900 GP |

</details>

## Reporting a correction

Include the category, brand, and model exactly as listed, the proposed change, and a public source. For regional names or aliases, include the market and explain how the names are related.

## Data license

A license for redistribution and reuse has yet to be selected.
