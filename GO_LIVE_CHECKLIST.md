# PatchitUP Franchise Application — Go-Live Checklist

---

## What's Been Built

### The Form
- [x] 11-step franchise application with splash page
- [x] 7-category competency assessment (56 questions)
- [x] Franchise Score (FRS) calculation engine
- [x] AI candidate analysis (pros, cons, training needs, unit recommendation)
- [x] Save progress (localStorage)
- [x] Admin panel with PDF report + email summary
- [x] Fully responsive (mobile + desktop)
- [x] PatchitUP branding, logo, Fira Sans, brand colors
- [x] GHL webhook fires on submission with all 52 fields

### GHL
- [x] 44 custom fields created under Opportunities
- [x] Inbound webhook configured and tested
- [x] Field mapping complete
- [x] Automation workflows built

### Email Templates
- [x] Admin notification email (with FRS scores, AI analysis, written responses)
- [x] Applicant confirmation email (branded, YouTube CTA, what happens next)

---

## To Go Live — 5 Steps

### Step 1 — Add email templates to GHL
1. Go to **Marketing → Emails → Templates**
2. Click **+ New Template** → select HTML editor
3. Paste the contents of `email-admin.html` → save as **"Franchise Application — Admin Notification"**
4. Repeat for `email-applicant.html` → save as **"Franchise Application — Applicant Confirmation"**

### Step 2 — Attach emails to your workflows
In your GHL workflows, find the "Send Email" action steps and attach:
- Admin email template to the admin notification step
- Applicant email template to the applicant confirmation step

### Step 3 — Add the form to your website
1. Log into WordPress
2. Go to Pages → open or create `/franchise-application`
3. Add a **Custom HTML** block
4. Paste the entire contents of `franchise-application.html` into the block
5. Set page template to **Full Width** (no sidebar)
6. Publish

### Step 4 — Send a live test submission
1. Go to `patchitupfranchise.com/franchise-application`
2. Complete the full form as a test applicant
3. Submit and verify:
   - [ ] Thank you screen appears
   - [ ] Admin email arrives in your inbox
   - [ ] Applicant confirmation email arrives
   - [ ] Contact + opportunity created in GHL
   - [ ] All 52 fields populated on the opportunity
   - [ ] Correct workflow triggered (Green/Yellow/Red)
   - [ ] Opportunity moves to correct pipeline stage

### Step 5 — Share the admin unlock code with your team
The admin panel on the thank-you screen is locked behind the code: **piu2024**

Share this only with your franchise development team. They use it after a submission to access:
- Full FRS score breakdown
- AI candidate analysis
- PDF report download
- Email summary button

---

## Files Reference

| File | Purpose |
|---|---|
| `franchise-application.html` | The form — paste into WordPress |
| `email-admin.html` | Admin email template — paste into GHL |
| `email-applicant.html` | Applicant email template — paste into GHL |
| `email-admin-preview.html` | Preview of admin email with sample data |
| `email-applicant-preview.html` | Preview of applicant email with sample data |
| `GHL_Custom_Fields_Guide_v2.md` | Reference for all 44 custom fields |
| `GHL_Webhook_Mapping.md` | All 52 field mappings for webhook |
| `webhook-test.html` | Test page to fire sample payload to GHL |

---

## Admin Unlock Code
**piu2024** — share with franchise development team only

## GHL Webhook URL
`https://services.leadconnectorhq.com/hooks/gN5lV0lMSTI7qdGs9YDJ/webhook-trigger/d626486f-1bdb-4973-a912-ab380d6edc14`

---

## Future Enhancements (when ready)
- Change admin unlock code from `piu2024` to something unique
- Add a PDF report hosting solution so the download link in the admin email works
- Build out the Yellow approval/denial email templates for candidates
- Add a nurture email sequence for Red and denied Yellow candidates
- Connect Airtable or Google Sheets as a backup application repository

