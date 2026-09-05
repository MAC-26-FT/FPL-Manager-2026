# Security

This is a static PWA. It does not request or store your FPL password, Apple ID, iCloud password, device passcode, financial data, contacts, photos or microphone access. It reads public FPL data and caches it in browser storage.

No software can honestly be guaranteed 100% secure. Use HTTPS-only hosting, a trusted domain, current iOS/iPadOS/macOS/Safari, and no third-party scripts. Never enter an FPL password into this app.

For production, use a strict Content-Security-Policy, X-Content-Type-Options: nosniff, Referrer-Policy: no-referrer and restrictive Permissions-Policy. Do not install profiles, certificates or extensions to use it.