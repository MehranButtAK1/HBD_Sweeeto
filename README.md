# For My Sweeto — Advanced Protected Birthday Website

This build uses browser-side AES-256-GCM encryption with PBKDF2 (200,000 iterations). The readable HTML, CSS, JavaScript and media assets are stored encrypted in `vault/`.

## Default password
**Sweeto@1509**

Change the password before sharing if you want a different secret. The password itself is not stored in the site; it is only used locally to derive the encryption key.

## Important security note
This is strong protection for a static GitHub Pages surprise, but it is not the same as server-side authentication. Because the decryption happens in the visitor's browser, a determined technical person can still attack the encrypted bundle offline. For true “only Roomi can access it” authentication, use a host/service with server-side access control (for example Cloudflare Access).

## GitHub Pages
1. Create a private GitHub repository if you also want the source repository private.
2. Upload the contents of this folder.
3. Enable GitHub Pages from the repository's Pages settings.
4. Share the Pages URL and the password only with Sweeto.

The site also includes `noindex,nofollow,noarchive` metadata, but this is not a security boundary.
