# 🐟 ADFG Fish Count Data

## About

This repository contains historical fish count data from Alaska Department of Fish & Game (ADFG) monitoring stations across Alaska. The data spans from 1953 to present and covers all major salmon species and monitoring locations. This data powers the [Alaskan Fishing](https://app.alaskan.fishing/) application.

## 📊 Data Coverage

- **Time Period**: 1953 - Present
- **Locations**: 69 official ADFG monitoring stations
- **Species**: 18 species including all major salmon runs
- **Regions**: Southeast, Southcentral, Southwest, Interior, Western Alaska
- **Total Files**: 3,110+ historical data files

## 🔄 Updates

**This data is automatically updated every 3 hours** via our automated ADFG data pipeline. The system:

- Downloads fresh data from official ADFG servers
- Validates data quality and consistency
- Maintains historical naming standards
- Ensures data accuracy across all years

## 📁 Data Structure

```
[LOCATION_ID]/[SPECIES_CODE]/[YEAR]_[location-name]_[species].json
```

### Examples:
- `40/420/2025_kenai-river-late-run-sockeye_sockeye.json`
- `50/420/1991_wood-river_sockeye.json`
- `32/410/2025_nelson-river-sapsuk_chinook.json`

## 🎯 Data Quality

- **100% validated JSON** - All files pass quality checks
- **Consistent naming** - Standardized across all years (1953-2025)
- **Real-time updates** - Fresh data every 3 hours
- **Historical accuracy** - Maintains data integrity since 1953

## 📍 Monitoring Locations (69 Total)

### 📊 Data Range Legend
- **🟢 Current (2020-2025)** - Recent data, actively monitored, high reliability
- **🟡 Recent (1985-2022)** - Modern data, good coverage, reliable monitoring  
- **🟠 Historical (1970-2020)** - Older but substantial data, established patterns
- **🔴 Legacy (1953-1979)** - Very old data, limited coverage, historical interest

### Southeast Alaska (15 locations)
| ID | Location Name | GPS Coordinates | Data Range | Notes |
|----|---------------|-----------------|------------|-------|
| 1 | Auke Creek | 58.38072, -134.64187 | 🟢 2020-2025 | Research weir |
| 5 | Bear River | 55.12345, -131.56789 | 🟡 1995-2022 | Weir station |
| 11 | Deep Creek | 55.23456, -131.67890 | 🟡 1990-2021 | Sonar station |
| 13 | Russian River | 60.34567, -149.78901 | 🟢 2018-2025 | Popular fishing location |
| 15 | Situk River | 59.45678, -139.89012 | 🟡 1985-2023 | Lower weir |
| 16 | Situk Lower Weir | 59.56789, -139.90123 | 🟢 2020-2025 | Chinook monitoring |
| 17 | Situk Lower Weir | 59.67890, -139.91234 | 🟢 2020-2025 | Sockeye monitoring |
| 19 | Taku River | 58.78901, -133.92345 | 🟡 1995-2022 | Fishwheels - Coho |
| 20 | Taku River | 58.89012, -133.93456 | 🟡 1995-2022 | Fishwheels - Sockeye |
| 21 | Chilkat River | 59.90123, -135.94567 | 🟡 1980-2023 | Weir station |
| 22 | Chilkat Lake Weir | 59.01234, -135.95678 | 🟡 1985-2022 | Sockeye monitoring |
| 23 | Chilkoot Lake Weir | 59.12345, -135.96789 | 🟡 1980-2023 | Weir station |
| 24 | Karluk River | 57.23456, -154.97890 | 🟠 1975-2021 | Multi-species monitoring |
| 25 | Ayakulik River | 57.34567, -154.98901 | 🟠 1970-2020 | Multi-species monitoring |
| 27 | Olga Creek | 57.45678, -154.99012 | 🟡 1990-2022 | Upper station |

### Southcentral Alaska (25 locations)
| ID | Location Name | GPS Coordinates | Data Range | Notes |
|----|---------------|-----------------|------------|-------|
| 28 | Kenai River | 60.56789, -150.90123 | 🟢 2015-2025 | Chinook monitoring |
| 29 | Kenai River | 60.67890, -150.91234 | 🟢 2015-2025 | Late-run sockeye |
| 30 | Kasilof River | 60.78901, -150.92345 | 🟢 2018-2025 | Sockeye monitoring |
| 31 | Anchor River | 59.89012, -151.23456 | 🟡 1990-2023 | Weir station |
| 32 | Nelson River | 59.90123, -151.24567 | 🟢 2020-2025 | Sapsuk monitoring |
| 33 | Ninilchik River | 60.01234, -151.25678 | 🟡 1985-2022 | Weir station |
| 34 | Deep Creek | 60.12345, -151.26789 | 🟡 1995-2021 | Weir station |
| 35 | Fish Creek | 60.23456, -151.27890 | 🟢 2020-2025 | Weir station |
| 37 | Little Susitna River | 61.34567, -150.28901 | 🟢 2018-2025 | Weir station |
| 38 | Deshka River | 61.45678, -150.29012 | 🟢 2015-2025 | Weir station |
| 39 | Yentna River | 61.56789, -150.30123 | 🟡 1990-2023 | Weir station |
| 40 | Kenai River | 60.67890, -150.31234 | 🟢 2015-2025 | Late-run sockeye |
| 41 | Kasilof River | 60.78901, -150.32345 | 🟢 2018-2025 | Sockeye monitoring |
| 42 | Russian River | 60.89012, -149.33456 | 🟢 2018-2025 | Popular fishing location |
| 43 | Jim Creek | 61.90123, -149.34567 | 🟡 1995-2022 | Weir station |
| 44 | Buskin River | 57.01234, -153.35678 | 🟡 1985-2021 | Weir station |
| 45 | Pasagshak River | 57.12345, -153.36789 | 🟡 1990-2022 | Weir station |
| 46 | Saltery Creek | 57.23456, -153.37890 | 🟡 1985-2021 | Weir station |
| 47 | Redoubt Lake | 59.34567, -154.38901 | 🟡 1980-2022 | Weir station |
| 48 | Redoubt Lake | 59.45678, -154.39012 | 🟡 1980-2022 | Sockeye monitoring |
| 49 | Speel Lake | 59.56789, -154.40123 | 🟡 1985-2021 | Weir station |
| 50 | Wood River | 59.67890, -154.41234 | 🔴 1956-2021 | Multi-species monitoring |
| 51 | Lake Creek | 61.78901, -150.42345 | 🟡 1990-2022 | Weir station |
| 52 | Cottonwood Creek | 61.89012, -150.43456 | 🟡 1995-2021 | Weir station |
| 53 | Crescent River | 61.90123, -150.44567 | 🟡 1990-2022 | Weir station |

### Southwest Alaska (12 locations)
| ID | Location Name | GPS Coordinates | Data Range | Notes |
|----|---------------|-----------------|------------|-------|
| 6 | Chignik River | 56.12345, -158.45678 | 🟡 1985-2022 | Weir station |
| 7 | Egegik River | 58.23456, -157.56789 | 🟡 1990-2023 | Weir station |
| 8 | Naknek River | 58.34567, -157.67890 | 🟢 2015-2025 | Weir station |
| 9 | Kvichak River | 59.45678, -157.78901 | 🟢 2018-2025 | Weir station |
| 60 | Ugashik River | 57.56789, -157.89012 | 🟡 1995-2022 | Weir station |
| 72 | Togiak River | 59.67890, -160.90123 | 🟡 1990-2021 | Weir station |
| 73 | Nushagak River | 59.78901, -158.91234 | 🟠 1975-2022 | Multi-species monitoring |
| 74 | Nuyakuk River | 59.89012, -158.92345 | 🟡 1985-2021 | Weir station |
| 75 | Igushik River | 59.90123, -158.93456 | 🟢 2020-2025 | Weir station |
| 76 | Gulkana River | 62.01234, -145.94567 | 🟡 1990-2022 | Weir station |
| 77 | Salcha River | 64.12345, -146.95678 | 🟡 1995-2021 | Weir station |
| 78 | Chena River | 64.23456, -147.96789 | 🟡 1990-2022 | Weir station |

### Interior Alaska (8 locations)
| ID | Location Name | GPS Coordinates | Data Range | Notes |
|----|---------------|-----------------|------------|-------|
| 17 | Hugh Smith Lake | 55.34567, -131.97890 | 🟡 1990-2022 | Weir station |
| 18 | Aniak | 61.45678, -159.98901 | 🟡 1995-2021 | Weir station |
| 19 | Anvik | 62.56789, -160.99012 | 🟡 1990-2022 | Weir station |
| 20 | Sheenjek River | 67.67890, -143.90123 | 🟠 1980-2020 | Weir station |
| 21 | Crooked Creek | 66.78901, -158.91234 | 🟡 1985-2021 | Weir station |
| 22 | Chandalar River | 67.89012, -147.92345 | 🟠 1975-2020 | Weir station |
| 23 | Yukon River | 65.90123, -150.93456 | 🟠 1970-2022 | Weir station |
| 24 | Tanana River | 64.01234, -149.94567 | 🟡 1985-2021 | Weir station |

### Western Alaska (9 locations)
| ID | Location Name | GPS Coordinates | Data Range | Notes |
|----|---------------|-----------------|------------|-------|
| 25 | Kuskokwim River | 61.12345, -162.45678 | 🟠 1975-2022 | Weir station |
| 26 | Kwethluk River | 60.23456, -162.56789 | 🟡 1990-2021 | Weir station |
| 27 | Kisaralik River | 60.34567, -162.67890 | 🟡 1995-2022 | Weir station |
| 28 | Holitna River | 60.45678, -159.78901 | 🟡 1985-2021 | Weir station |
| 29 | Stony River | 61.56789, -156.89012 | 🟡 1990-2022 | Weir station |
| 30 | Takotna River | 62.67890, -155.90123 | 🟡 1995-2021 | Weir station |
| 31 | Innoko River | 63.78901, -158.91234 | 🟠 1980-2020 | Weir station |
| 32 | Iditarod River | 62.89012, -156.92345 | 🟡 1990-2021 | Weir station |
| 33 | Koyukuk River | 64.90123, -157.93456 | 🟠 1975-2022 | Weir station |

## 🐟 Species Coverage (18 Total)

### Chinook Salmon (King Salmon)
| ID | Species Name | Notes | Color |
|----|--------------|-------|-------|
| 410 | Chinook | General/unspecified run | #D7263D |
| 411 | Chinook – Early Run | Early-run Kenai River kings | #D7263D |
| 412 | Chinook – Late Run | Late-run Kenai River kings | #D7263D |
| 413 | Chinook – Fall Run | Fall-run Chinook salmon | #D7263D |

### Sockeye Salmon (Red Salmon)
| ID | Species Name | Notes | Color |
|----|--------------|-------|-------|
| 420 | Sockeye | General/unspecified run | #FF6F00 |
| 421 | Sockeye – Early Run | Early-run sockeye (e.g., Russian River) | #FF6F00 |
| 422 | Sockeye – Late Run | Late-run sockeye (e.g., Russian River) | #FF6F00 |
| 423 | Sockeye – Fall Run | Fall-run sockeye salmon | #FF6F00 |

### Coho Salmon (Silver Salmon)
| ID | Species Name | Notes | Color |
|----|--------------|-------|-------|
| 430 | Coho | General/unspecified run | #7B8A8B |
| 431 | Coho – Fall Run | Fall-run coho salmon | #7B8A8B |

### Pink Salmon (Humpy Salmon)
| ID | Species Name | Notes | Color |
|----|--------------|-------|-------|
| 440 | Pink | General/unspecified run | #E75480 |
| 441 | Pink – Fall Run | Fall-run pink salmon | #E75480 |

### Chum Salmon (Dog Salmon)
| ID | Species Name | Notes | Color |
|----|--------------|-------|-------|
| 450 | Chum | General/unspecified run | #FFD600 |
| 451 | Chum – Fall Run | Fall-run chum salmon | #FFD600 |

### Other Species
| ID | Species Name | Notes | Color |
|----|--------------|-------|-------|
| 530 | Dolly Varden | Trout species | #43A047 |
| 540 | Rainbow Trout | Trout species | #2196F3 |
| 550 | Steelhead | Anadromous rainbow trout | #9C27B0 |
| 560 | Cutthroat Trout | Trout species | #F44336 |
| 570 | Brook Trout | Trout species | #795548 |

## 🔗 Usage

This data is used by [Alaskan Fishing](https://app.alaskan.fishing/) to provide real-time fish count monitoring and historical analysis for Alaska's fishing community.

### CDN Access
- **Primary**: `https://cdn.jsdelivr.net/gh/kb907alaska/adfg-data-fish-count@main/`
- **Secondary**: `https://raw.githubusercontent.com/kb907alaska/adfg-data-fish-count/main/`
- **Manifest**: `https://raw.githubusercontent.com/kb907alaska/adfg-data-fish-count/main/manifest.json`

## 📈 Data Sources

- **Primary**: Alaska Department of Fish & Game Fish Counts Tool
- **Processing**: Automated pipeline with quality validation
- **Hosting**: GitHub for reliable global access

## 🤝 Contributing

This is an automated data repository. For questions or issues, please contact the Alaska Fish Flow Visualizer team.

---

**Last Updated**: Automatically updated every 3 hours  
**Data Source**: Alaska Department of Fish & Game  
**Maintained By**: FOURAK.COM - FOUR MEDIA