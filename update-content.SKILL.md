# update-content

## Description
Automates bulk updates of contact information, domain URLs, service descriptions, and other customizable content in the static HTML landing page. This skill streamlines deployment preparation by handling multiple replacements across the file, reducing manual errors and ensuring consistency.

## When to Use
- Before deployment: Update hardcoded phone numbers, emails, domain URLs
- Content customization: Change service descriptions, company name, addresses
- SEO updates: Modify meta tags, schema.org data
- Integration setup: Configure Formspree, Calendly, HubSpot endpoints

## Workflow
1. **Inventory current values**: Use grep_search to find common placeholder patterns (phone numbers, emails, domains, service text)
2. **Prompt for updates**: Ask user for new values for each category (phone, email, domain, etc.)
3. **Validate inputs**: Ensure formats are correct (e.g., valid email, URL)
4. **Bulk replace**: Use replace_string_in_file to update all occurrences, preserving context
5. **Verify changes**: Run a quick grep to confirm replacements and check for any missed instances

## Common Patterns to Update
- Phone: `+52-222-XXX-XXXX` or `+522221234567`
- Email: `contacto@premium.com`
- Domain: `https://tudominio.com/`
- Calendly: `calendly.com/tuusuario/30min`
- Formspree: `https://formspree.io/f/YOUR_FORM_ID`
- Company name: "Premium Services" or "Servicios Premium Puebla"
- Service descriptions: Look for Spanish text blocks in service sections

## Pitfalls
- Ensure all occurrences are updated (use case-insensitive search if needed)
- Preserve HTML structure and attributes during replacements
- Test links and forms after updates
- Backup the file before bulk changes

## Example Usage
When user requests "update contact info", invoke this skill to systematically replace all placeholders with user-provided values.</content>
<parameter name="filePath">c:\Users\gumod\Documents\Dev\Projects\MultiConstrucciones\update-content.SKILL.md