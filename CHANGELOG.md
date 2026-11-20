# Changelog

## v1.0.0 (2026-11-09)

- First release of the free Typeform GTM listener.
- Fires `typeform_form_submit` on Typeform's `form-submit` message and `typeform_form_start` on `form-started`, from every embed type.
- Trusts only `*.typeform.com`, including older yourname.typeform.com links.
- Ignores null, text and other junk messages without errors.
- One push per response ID, also when the message arrives twice or the GTM tag fires twice.
- Reads the form ID from the iframe address when the message has none.
- Own event names, so it never mixes with GA4's automatic form_submit and form_start.
