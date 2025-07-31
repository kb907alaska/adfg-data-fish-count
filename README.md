# Alaska Fish Count Data

## 🐟 **About This Repository**

This repository contains **public fish count data** from the Alaska Department of Fish and Game (ADFG). The data is automatically updated and provides real-time access to salmon and other fish counts across Alaska's monitoring stations.

## 📊 **Data Source**

- **Source**: [Alaska Department of Fish and Game Fish Counts](https://www.adfg.alaska.gov/sf/FishCounts/)
- **Update Frequency**: Every 30 minutes during fishing season
- **Coverage**: 69 monitoring stations across Alaska
- **Species**: Chinook, Sockeye, Coho, Pink, Chum, and Steelhead

## 📁 **Data Structure**

```
adfg-data-fish-count/
├── [LOCATION_ID]/              # Location folders (1, 5, 13, etc.)
│   └── [SPECIES_ID]/           # Species folders (410, 420, etc.)
│       └── [YEAR]_[location]_[species].json
├── manifest.json               # File index and metadata
└── logs/                       # Update logs
```

### **File Naming Example**
```
5/410/2025_situk-river_chinook.json
```

### **Data Format**
```json
{
  "DATA": [
    [2025, "2025-07-01", 1250],
    [2025, "2025-07-02", 1340]
  ],
  "last_updated": "2025-07-31T12:00:00Z"
}
```

## 🌐 **Accessing the Data**

### **Direct Access**
```
https://raw.githubusercontent.com/kb907alaska/adfg-data-fish-count/main/
```

### **CDN Access**
```
https://cdn.jsdelivr.net/gh/kb907alaska/adfg-data-fish-count@main/
```

### **Example File**
```
https://raw.githubusercontent.com/kb907alaska/adfg-data-fish-count/main/5/410/2025_situk-river_chinook.json
```

## 📍 **Geographic Coverage**

### **Regions**
- **Southeast Alaska**: Situk River, Russian River, Chilkat River
- **Southcentral Alaska**: Kenai River, Kasilof River, Anchor River
- **Interior Alaska**: Chena River, Salcha River, Gulkana River
- **Southwest Alaska**: Buskin River, Pasagshak River, Egegik River
- **Western Alaska**: Yukon River, Kvichak River, Naknek River

### **Species Monitored**
- **Chinook Salmon** (King Salmon)
- **Sockeye Salmon** (Red Salmon)
- **Coho Salmon** (Silver Salmon)
- **Pink Salmon** (Humpy Salmon)
- **Chum Salmon** (Dog Salmon)
- **Steelhead Trout**

## 📈 **Data Features**

- **Real-time Updates**: Data refreshed every 30 minutes
- **Historical Data**: Records dating back to the 1950s
- **Seasonal Coverage**: Full fishing season monitoring
- **Public Access**: No authentication required
- **CDN Optimized**: Fast global delivery

## 🔄 **Automated Updates**

This repository is automatically maintained through secure GitHub Actions workflows that:
- Fetch fresh data from ADFG
- Validate data quality
- Update files in real-time
- Maintain data integrity

## 📞 **Support**

For questions about:
- **Data Access**: Use the CDN URLs above
- **File Structure**: Check the manifest.json file
- **Technical Issues**: Contact repository maintainers

---

**🎯 This repository provides clean, reliable access to Alaska's fish count data for researchers, developers, and the public.**

*Data provided by the Alaska Department of Fish and Game* 