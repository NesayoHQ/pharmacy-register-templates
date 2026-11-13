# Pharmacy register templates: H1, expiry, purchase (blank, CC0)

H1 register format kaise banaye? Teen khali register, Excel aur CSV mein, har column ka naam English aur Hindi dono mein. Sign-up nahi, email nahi, kuch install nahi karna.

Three blank registers for an Indian retail pharmacy, as CSV and Excel. Each column heading is in English and Hindi in the same cell. No sign-up, no email, nothing to install.

| File | What it is |
|---|---|
| [`h1-register.xlsx`](h1-register.xlsx) / [`.csv`](h1-register.csv) | Schedule H1 supply register, one row per supply |
| [`expiry-register.xlsx`](expiry-register.xlsx) / [`.csv`](expiry-register.csv) | Expiry check list. The Excel file works out the last day of sale from the printed month |
| [`purchase-register.xlsx`](purchase-register.xlsx) / [`.csv`](purchase-register.csv) | Stock received, batch by batch, with the supplier's bill number |

## Worked example 1: expiry (invented data)

The pack is printed `08/2026`. Type that in the "Expiry printed" column, as text. The Excel file fills the next column:

| S. No. | Medicine | Batch no. | Expiry printed | Last day of sale |
|---|---|---|---|---|
| 1 | Example Tablet 10 strip | EX1234 | 08/2026 | 31/08/2026 |

The formula in the "Last day of sale" column reads the month and year, and returns the last day of that month. The full formula is in the file.

Why: Drugs and Cosmetics Rules, 1945, Rule 96, Explanation: "the date of expiry shall be in terms of month and year and it shall mean that the drug is recommended till the last day of the month." A pack printed 08/2026 can be sold through 31 August 2026, not only until 1 August.

## Worked example 2: Schedule H1 (all names and the address are invented)

| S. No. | Date of supply | Patient name | Patient address | Prescriber name | Prescriber address | Drug name | Quantity |
|---|---|---|---|---|---|---|---|
| 1 | 05/08/2026 | Patient A | 12 Example Road, Example Town | Dr. B | Example Clinic, Example Town | Example Drug 10 mg tablet | 10 |

The remaining columns (manufacturer, batch no., expiry, bill no., pharmacist signature) are in the file.

## Where the columns come from

Two separate duties are involved. This template has the columns for both, but a filled-in sheet is not proof that either duty is met.

1. The separate H1 register. Rule 65(3)(h), as published in the Rules: "the supply of a drug specified in Schedule H1 shall be recorded in a separate register at the time of the supply giving the name and address of the prescriber, the name of the patient, the name of the drug and the quantity supplied and such records shall be maintained for three years and be open for inspection."
2. The prescription register or serially numbered cash or credit memo. Rule 65(3)(1)(a)-(g) lists what that record carries: serial number, date of supply, name and address of the prescriber, name and address of the patient, the drug and quantity, and, for Schedule C, H and H1 drugs, the manufacturer's name, batch number and date of expiry, and the registered pharmacist's signature.

Source text: Rule 65 of the Drugs and Cosmetics Rules, 1945, as published at indiankanoon.org/doc/147665881. Check the current Gazette text before you rely on any of it.

## Expiry and Rule 65(17)

Rule 65(17): "No drug shall be sold or stocked by the licensee after the date of expiration of potency recorded on its container, label or wrapper, or in violation of any statement or direction recorded on such container, label or wrapper". The proviso lets a licensee who has taken steps with the manufacturer for withdrawal, reimbursement or disposal keep such drugs, stored separately from trade stock in packages or cartons marked "Not for sale". The expiry register has an Action column for that decision.

## Limits

- These are layouts, not legal advice and not an official format. Check them with your drug inspector or your CA before you rely on them.
- The purchase register is a working record, not a statutory format.
- Nothing here contains real patient, shop or customer data. Do not add any to a public copy.
- Licence: CC0 1.0. Use, change and share freely.

## More

A batch-wise stock register template (opening, received, sold, closing quantity) is on the Nesayo site: https://nesayo.com/tools/pharmacy-stock-register-format?utm_source=github&utm_medium=readme&utm_campaign=register_templates_2026_10&utm_content=register-templates-readme

Team Nesayo makes billing, stock and compliance software for Indian pharmacies. Nesayo fits a single medical store that wants billing free forever, in the browser on any phone or computer. Questions or corrections: open an issue, or write to hello@nesayo.com.
