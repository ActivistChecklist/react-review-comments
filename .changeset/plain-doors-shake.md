---
"@activistchecklist/react-review-comments": patch
---

Declare `next` as a peer dependency (`^14 || ^15 || ^16`) instead of a hard dependency.

Consuming apps now satisfy it with the Next.js version they already install, so the package
no longer pins (or nests) its own copy of `next`. This also means a Next.js security patch in
the host app applies to this package immediately, with no release here required.
