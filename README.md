# Fabric-Automated-Data-

┌────────────────────┐
│ Source CSV          │
│ Employee Attrition  │
└─────────┬──────────┘
          ↓
┌────────────────────┐
│ Lakehouse Files     │
│ /Files/raw/         │
└─────────┬──────────┘
          ↓
┌────────────────────┐
│ 01_Bronze_Load      │
│ Notebook            │
│ Creates/overwrites  │
│ bronze_employee     │
└─────────┬──────────┘
          ↓
┌────────────────────┐
│ 02_Silver_Transform │
│ Notebook            │
│ Cleans, types,      │
│ standardizes data   │
└─────────┬──────────┘
          ↓
┌────────────────────┐
│ 03_Gold_Aggregations│
│ Notebook            │
│ Creates business    │
│ metric tables       │
└─────────┬──────────┘
          ↓
┌────────────────────┐
│ Semantic Model      │
│ Refresh             │
└─────────┬──────────┘
          ↓
┌────────────────────┐
│ Power BI Reports    │
│ Workforce Overview  │
│ Attrition Drivers   │
└────────────────────┘
