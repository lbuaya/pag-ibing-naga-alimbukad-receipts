ATENEO BLUE BAND RECEIPT SYSTEM
================================

An offline receipt and verification system for The Ateneo Blue Band.
Allows finance officers to generate, print, and verify official receipts.
Hosted on GitHub Pages for easy and secure use.

--------------------------------
LIVE LINKS
--------------------------------
Main Link:
https://abbfinance.github.io/receipts/

Generate Receipt:
https://abbfinance.github.io/abb/Ateneo_Blue_Band_Receipt_Generator.html

Verify Receipt:
https://abbfinance.github.io/abb/verify.html

--------------------------------
HOW TO USE
--------------------------------

RECEIPT GENERATION
------------------
1. Open “Ateneo_Blue_Band_Receipt_Generator.html” in your browser.
2. Fill in the name, grade & section, email, payment type, invoice number, and date.
3. Add as many items as needed using the “+ Add Item” button.
4. Click “Done (Fill Template)” to generate a printable preview.
5. Check the details, then click “Print Receipt”.

When printed, a new “valid_invoices.json” file will automatically download.
→ Replace your old valid_invoices.json with the new one to keep it updated.

Each new printed receipt is automatically recorded in the JSON file.
The invoice number will then be recognized as a valid transaction.

⚠️ MAKE SURE TO PRINT THE RECEIPT FIRST BEFORE DOWNLOADING THE JSON!

--------------------------------
DOWNLOADING THE UPDATED JSON
--------------------------------
You can also click the “Download Updated valid_invoices.json” button anytime
to manually save your updated list of invoice numbers.

--------------------------------
VERIFYING RECEIPTS
--------------------------------
1. Open “verify.html” in your browser.
2. It will automatically load “valid_invoices.json” if it’s in the same folder.
3. If it cannot read it automatically (for example, when opened via file://),
   click the “Choose File” button and manually select your valid_invoices.json.
4. Type or scan the invoice number from a printed receipt.

If the invoice exists in the JSON file, you’ll see:
   ✅ VALID RECEIPT
Otherwise, it will show:
   ❌ NOT FOUND OR INVALID

--------------------------------
JSON FILE FORMAT
--------------------------------
The “valid_invoices.json” file uses this format:

{
  "valid_invoices": [
    "INV-2025-001",
    "INV-2025-002",
    "INV-2025-003"
  ]
}

Keep this file in the same folder as your HTML files
to ensure the verifier can detect valid receipts.

--------------------------------
CREATED FOR
--------------------------------
The Ateneo Blue Band  
Finance Office | 2025
