# KG integration test data

### Repo Structure
- _snippets: for each tool of kg tools a snippet for testing
- $DATASET_NAME: name of the dataset independent of the tool, this is not an example but a real benchmark dataset

Create dir/.keep 

---
### $NAME

Domain: ${Medical Data, Cross, Geographical, Financial, ...}

Description: ${A short text describing the dataset usage}

Format: ${mime-type: text/turtle, application/ntriples, application/json, text/plain}

Metadata: ${byte size, schema}

DownloadLink:

PaperName:

Structure: $(tree)

---
### AbtBuy

Domain: products (consumer electronics and home appliances)

Description: Abt

    subject_id: A unique identifier for each product.
    
    name: The product's name, often including the brand and model.
    
    description: Detailed product specifications and features.
    
    price: The cost of the product (though not consistently filled in).
    
Metadata:
- Schema:
  
  ```
     subject_id=number
     name= text
     description= text
     price= decimal
  ```
- matches: 1097

Structure:

```
.
└── record_descriptions
    ├── 1_abt.csv
    └── 2_buy.csv

1 directory, 2 files
```
