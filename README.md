# ADFG Fish Count Data Repository

## 🎯 **Purpose**

This repository contains **public fish count data** from the Alaska Department of Fish and Game (ADFG) Fish Counts Tool. The data is automatically updated via secure GitHub Actions workflows.

## 🔒 **Security Architecture**

### **Repository Structure**
- **This Repository** (`[kb907alaska/adfg-fishcount](https://github.com/kb907alaska/adfg-data-fish-count)`): **Public** - Contains only JSON data files

### **Why This Architecture?**
- ✅ **Public Data Access**: JSON files are publicly accessible for CDN delivery

## 📊 **Data Source**

All data is automatically collected from:
- **Source**: [ADFG Fish Counts Tool](https://www.adfg.alaska.gov/sf/FishCounts/index.cfm)
- **Method**: Automated web scraping via GitHub Actions
- **Frequency**: Every 30 minutes during fishing season
- **Coverage**: 29 valid location-species combinations across Alaska

## 📁 **Data Structure**

```
adfg-fishcount/
├── README.md                    # This file
├── manifest.json               # File index and metadata
├── [LOCATION_ID]/              # Location folders (5, 9, 13, etc.)
│   └── [SPECIES_ID]/           # Species folders (410, 420, etc.)
│       └── [YEAR]_[location]_[species].json
└── ... (29 valid combinations)
```

### **File Naming Convention**
```
{year}_{location-name}_{species}.json
Example: 2025_russian-river_sockeye-early-run.json
```

### **JSON Data Format**
```json
{
  "LOCATION_ID": "13",
  "SPECIES_ID": "421", 
  "YEAR": 2025,
  "DATA": [
    [1, "2025-07-01", 1250],
    [2, "2025-07-02", 1340]
  ],
  "last_updated": "2025-07-30T12:00:00Z"
}
```

## 🔄 **Update Process**

### **Automated Updates**
1. **Update Workflow**: Runs every 30 minutes
2. **Data Collection**: Fetches fresh data from ADFG website
3. **File Updates**: Updates JSON files in this repository
4. **CDN Delivery**: Files immediately available via GitHub CDN

### **Manual Updates**
- **Force Update**: Trigger workflow with `force_update: true`
- **Target Year**: Specify year with `target_year: "2025"`
- **Manual Trigger**: Via GitHub Actions UI

## 🌐 **CDN Access**

### **Primary URLs**
```
https://raw.githubusercontent.com/kb907alaska/adfg-fishcount/main/
https://cdn.jsdelivr.net/gh/kb907alaska/adfg-fishcount@main/
```

### **Example File Access**
```
https://raw.githubusercontent.com/kb907alaska/adfg-fishcount/main/13/421/2025_russian-river_sockeye-early-run.json
```

## 📈 **Data Coverage**

### **Locations (29 combinations)**
- **Southeast**: Situk River, Russian River, etc.
- **Southcentral**: Kenai River, Kasilof River, etc.
- **Interior**: Chena River, Salcha River, etc.
- **Southwest**: Buskin River, Pasagshak River, etc.

### **Species**
- **Chinook Salmon** (410, 411, 412)
- **Sockeye Salmon** (420, 421, 422)
- **Coho Salmon** (430)
- **Pink Salmon** (440)
- **Chum Salmon** (450)
- **Steelhead Trout** (540)

### **Time Range**
- **Historical**: Data back to 1950s
- **Current**: 2025 season data
- **Updates**: Real-time during fishing season

## 🛡️ **Security Notes**

### **What's Public**
- ✅ JSON fish count data files
- ✅ README documentation
- ✅ Manifest file (file index)

## 📞 **Support**

For questions about:
- **Data**: Check this README and file structure
- **Workflows**: Contact repository maintainers
- **Access**: Use CDN URLs above

---

**🎯 This repository provides clean, public access to ADFG fish count data while maintaining security through private automation workflows.** 
