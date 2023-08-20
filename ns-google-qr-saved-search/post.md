# 🚀 NetSuite QR Code Generator

This repository contains a formula for generating QR code images in NetSuite saved searches. With this formula, you can easily create QR codes based on field values, such as `{entitystatus}`.

## 📋 Usage

1. Copy the formula provided below.

2. Create a new formula text field in your NetSuite saved search.

3. Paste the formula into the newly created text field.

4. Replace `{entitystatus}` with the field you want to encode as a QR code.

5. Save and run the saved search. QR code images will be generated based on the field values.

## Formula Text

```sql
'<img src="https://chart.googleapis.com/chart?chs=200x200&cht=qr&chl=' || {entitystatus} || '&choe=UTF-8">'
```

## 💡 Example

Here's an example of how the formula can be used in your NetSuite saved search to generate QR codes:

```sql
'<img src="https://chart.googleapis.com/chart?chs=200x200&cht=qr&chl=' || {entitystatus} || '&choe=UTF-8">'
```

Feel free to customize the QR code size and encoding field to suit your needs.

Happy QR code generating! 📦🔍📷
