# Opencart's Journal v3x Rich Snippets Language Fix
Created an OCMOD modification file to fix the language-specific JSON-LD structured data issue in the Journal3 theme.

### File created:
- `knns_journal3_rich_snippets_language_fix.ocmod.xml`

### Fixes implemented:
1. Product URL fix
2. Product description fix
3. Site description fix

### Installation instructions:
1. Upload the file: 
   - `/system/knns_journal3_rich_snippets_language_fix.ocmod.xml`
2. OpenCart Admin:
   - Go to Extensions → Modifications
   - Click the refresh button (circular arrow icon) to refresh modifications
   - The OCMOD will be automatically detected and applied
3. Clear cache:
   - Go to Dashboard → Settings → Developer Settings
   - Clear modification cache
   - Clear theme cache (if available)
4. Verify:
   - Visit a product page in each language (Greek, English, Italian etc)
   - View page source and check the JSON-LD structured data
   - Verify that:
     - The `url` field matches the current page URL
     - The `description` field shows content in the correct language
     - The WebSite schema `description` is in the correct language
