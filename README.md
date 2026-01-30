# ECOS Technologies Website - Complete Package

## Files Included

### Original Pages (Updated)
- `index.html` - Homepage
- `services.html` - Services overview
- `industries.html` - Industries overview (updated with new links)
- `compliance.html` - Certifications & compliance
- `process.html` - How it works
- `resources.html` - Pricing & resources (updated with tool links)
- `about.html` - About ECOS
- `contact.html` - Contact form

### NEW Industry Landing Pages
- `healthcare.html` - Healthcare ITAD (HIPAA focus)
- `financial.html` - Financial Services (SOX/GLBA focus)
- `government.html` - Government (NIST/DoD focus)
- `data-center.html` - Data Center Decommissioning

### NEW Interactive Tools
- `value-estimator.html` - Equipment value calculator
- `esg-calculator.html` - Environmental impact calculator
- `quick-quote.html` - Fast lead capture form

### NEW Lead Magnets
- `sample-cod.html` - Gated Sample Certificate of Destruction
- `sample-cod-gated.html` - Same as above (backup)
- `hipaa-checklist.html` - HIPAA Disposal Checklist download
- `vendor-scorecard.html` - ITAD Vendor Evaluation Scorecard

### NEW Trigger Event Pages
- `ma-itad.html` - M&A IT Disposition
- `office-relocation.html` - Office Move IT Disposal

---

## Deployment to Netlify

1. Upload all files to your Netlify site
2. Create `_redirects` file with:
```
/industries/healthcare  /healthcare  301
/industries/financial   /financial   301
/industries/government  /government  301
/industries/education   /data-center 301
```

---

## Integration Changes Made

### industries.html
- Healthcare link → `/healthcare`
- Financial link → `/financial`
- Government link → `/government`
- Footer updated with new industry pages

### resources.html
- Added Value Estimator link to nav tabs
- Added ESG Calculator link to nav tabs
- Sample COD now points to gated version

---

## Form Setup Required

All forms use Formspree. Replace `YOUR_FORM_ID` with your Formspree form ID in:
- `quick-quote.html` (line ~95)
- `sample-cod.html` / `sample-cod-gated.html` (line ~456)
- `hipaa-checklist.html` (form action)
- `vendor-scorecard.html` (form action)

Your existing Formspree ID: Check your current contact.html for the ID

---

## Cold Email → Landing Page Mapping

| Email Campaign | Landing Page | URL |
|---------------|--------------|-----|
| Healthcare IT Directors | Healthcare | `/healthcare` |
| Financial Compliance | Financial | `/financial` |
| Government IT Managers | Government | `/government` |
| Data Center Ops | Data Center | `/data-center` |
| M&A IT Teams | M&A ITAD | `/ma-itad` |
| Office Relocations | Office Move | `/office-relocation` |
| General Quick Quote | Quick Quote | `/quick-quote` |

---

## Tracking Parameters

All CTAs pass source parameters for analytics:
- `?source=healthcare`
- `?source=financial`
- `?source=government`
- `?source=datacenter`
- `?source=ma`
- `?source=relocation`
- `?source=estimator`

---

## Lead Magnet PDFs Needed

Create these PDFs to complete the gated content:
1. `/downloads/hipaa-disposal-checklist.pdf`
2. `/downloads/itad-vendor-scorecard.xlsx`

---

## Testing Checklist

- [ ] All nav links work
- [ ] Forms submit to Formspree
- [ ] Value estimator calculates correctly
- [ ] ESG calculator works
- [ ] Mobile responsive on all pages
- [ ] Contact page receives source parameters
- [ ] All images load correctly

---

## Questions?

All pages use your existing:
- Logo URL
- Color scheme (#00539C primary, #5CB85C success)
- Inter font family
- Footer structure
- Header navigation pattern
