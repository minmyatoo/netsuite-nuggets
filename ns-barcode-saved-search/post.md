📊 Barcode Generation in NetSuite Saved Search

📦 This repository contains a NetSuite saved search formula to generate barcodes using the JsBarcode library. The saved search formula text provided here can be used to generate barcode images in NetSuite based on the `internalid` field.

## 🚀 Getting Started

### 📋 Prerequisites

Before using this formula, make sure you have the following prerequisites in place:

- 🔐 Access to a NetSuite account.
- 🧠 Basic knowledge of NetSuite saved searches.
- 🌐 Internet connectivity to load the JsBarcode library from a CDN.

### 📝 Usage

1. 📋 Copy the provided formula text and create a new formula text field in your NetSuite saved search.

2. 📄 Paste the formula text into the newly created formula text field.

3. 📂 Ensure that you have a field in your saved search named `{internalid}` that contains the data you want to encode as a barcode.

4. 💾 Save and run the saved search. You should see barcode images generated based on the `internalid` field for each row in the search results.

### 🌟 Example

Here's an example of the formula text to be used in your NetSuite saved search:

```sql
CASE
    WHEN rownum = 1 THEN
        '<script src="https://cdn.jsdelivr.net/npm/jsbarcode@3.11.0/dist/barcodes/JsBarcode.code128.min.js"></script>'
    ELSE
        '<svg id="barcode' || rownum || '"></svg><script>JsBarcode("#barcode' || rownum || '", "' || {internalid} || '");</script>'
END
```

Feel free to use this emoji-enhanced post as you like! 😊👍
