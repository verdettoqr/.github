# Security policy

This policy covers everything published under the verdettoqr account: the Verdetto Android app, the
link-safety-list pipeline and the bundle it publishes, and the verdettoqr.com site.

## Reporting a vulnerability

Please report privately, not in a public issue:

- through GitHub's private vulnerability reporting on the repository concerned (Security tab, "Report a
  vulnerability"), or
- by email to support@verdettoqr.com.

Include what you found, how to reproduce it, and what you think it allows. You will get an acknowledgement
within a few days and a plain answer about what happens next. There is no bounty program; credit in the fix's
notes is offered if you want it.

## What matters most

- Anything that makes the app open, join, dial, or send something without the person's own tap.
- Anything that lets a scanned code or a lookup answer run code, read history, or leave the phone.
- A way to publish or accept an unsigned or tampered safety bundle: the app verifies the manifest's signature
  and every asset's hash before use, and the signing key never leaves the pipeline's secrets.
- Anything on the site that is not a static page.

## Out of scope

- The app saying "No warnings found" for a link that turns out to be harmful. The app never claims anything is
  safe; a missed entry is a data gap to report to the source list, not a vulnerability.
- The services the app can ask when online lookups are on (Open Food Facts, Open Library, the national
  libraries, openFDA, MusicBrainz, Wikidata, the NHTSA database, rdap.org, GitHub). Report those to their owners.

## Supported versions

The current release on Google Play and the current safety bundle (the rolling `current` release). Older
bundles are replaced, never patched.
