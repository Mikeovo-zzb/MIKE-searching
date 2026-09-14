# Privacy and repository-export checklist

Use this checklist before committing or sharing the skill.

## Keep

- generalized workflow, score definitions, decision gates, message structure, follow-up logic, generic schemas, and de-identified lessons;
- public-safe FlavorWise product terminology and links;
- placeholders such as `[Company]`, `[Name]`, `[Market]`, `[Content Anchor]`, and `[Next Action]`.

## Remove

- customer, creator, media, distributor, retailer, dealer, or grower names;
- personal names, emails, phone numbers, addresses, social handles, account IDs, and private URLs;
- Gmail or WhatsApp message text, screenshots, attachments, and private conversation details;
- shipping destinations, order numbers, device IDs, credentials, invoices, private proposals, and account histories;
- customer-specific prices, discounts, freight, taxes, payment terms, territory, exclusivity, warranty exceptions, or internal margins;
- current pipeline stages, next actions, forecast values, private objections, and outcome data tied to an identifiable party;
- Any project-external customer context or named customer.

## Scrub test

Search the package for names, email-like strings, phone-like strings, street addresses, order/device IDs, and unique client phrases. Replace each with a role or placeholder. A reader who has never seen the source project should be unable to reconstruct a client identity or deal.

## Runtime rule

When the skill is used with a real object, private data may be supplied for the immediate task if the user authorizes it. Keep it in the active working context only; do not copy it into the skill, reusable examples, public repository, or generalized learning without explicit permission and de-identification.
