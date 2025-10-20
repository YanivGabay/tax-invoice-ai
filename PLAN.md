# Tax Invoice AI - Project Plan

## Sample Input/Output

### RECEIPT A:
```
Date: 15/6/25
ID: 1515151515

Items:
- 5kg banana - price 150
- 3kg apple - price 120
```

### EXPECTED OUTPUT:
```
Date: 15/6/25
Invoice ID: 1515151515
Total Weight: 8kg
Total Price: 270
Items: banana, apple
```

## Project Approach

### Phase 1: Local Script Development

**Objective**: Create a basic Python script that processes invoice images from local folders

**Input Structure**:
```
invoices/
├── client_1/
│   ├── invoice_001.jpg
│   ├── invoice_002.pdf
│   └── invoice_003.png
├── client_2/
│   ├── invoice_001.jpg
│   └── invoice_002.pdf
└── output/
    ├── client_1_results.json
    └── client_2_results.json
```

**Core Features**:
- Process images/PDFs from client folders
- Extract key information using AI/OCR
- Generate structured output files

**Information to Extract**:
- Invoice Number
- Date
- Total amount/weight of items
- Total price
- Item descriptions/categories
- Country of origin (if available)

**Technology Stack**:
- Python (core processing)
- OCR library (text extraction)
- AI/ML model (information parsing)
- File I/O handling

**Workflow**:
1. Scan client folders for invoice files
2. Process each image/PDF
3. Extract text using OCR
4. Parse information using AI
5. Save results to JSON/CSV files
6. Generate summary reports