# Elite Medical Clinic Website

Pure HTML5 + CSS3 + Vanilla JavaScript frontend. Google Sheets + Google Apps Script are used only for backend storage/submissions.

## Important source verification

The supplied Google Maps short link currently appears to resolve to a different business/location than the expected Elite Medical Clinic. Do not publish its address, phone or location as verified until the clinic confirms it.

The supplied Instagram profile was not reliably accessible to the automated fetch, so no private/unverified Instagram content was copied.

## Setup

1. Open `script.js` and replace only verified clinic data.
2. Create a dedicated Google Sheet.
3. Open Extensions → Apps Script.
4. Paste `code.gs`.
5. Replace `PASTE_GOOGLE_SHEET_ID_HERE` with the Sheet ID.
6. Deploy → New deployment → Web app.
7. Execute as: Me.
8. Access: Anyone.
9. Copy the `/exec` URL.
10. Put it into `config.js` as `APPS_SCRIPT_URL`.
11. Upload the frontend to static hosting.

## Sheet columns

Timestamp | FormType | Name | Email | Phone | Service | Date | Time | Message | Source | PageURL

## Test

Submit an appointment and a contact inquiry. Confirm each creates a new row in `Leads`. Also test invalid input and backend failure.

Never put Google credentials or private keys in frontend files.
