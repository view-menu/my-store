# Restaurant menu: admin creates, customers view

| Page | Who | Link |
|---|---|---|
| Customer menu | Customers (QR code) | `https://<username>.github.io/<repo>/` |
| Admin | Restaurant staff only | `https://<username>.github.io/<repo>/admin.html` |

## One-time setup
1. Create a GitHub repository and upload all files from this folder to its root.
2. Settings → Pages → Deploy from a branch → `main`, `/ (root)` → Save.
3. Create an access token: GitHub → Settings → Developer settings → Fine-grained tokens → Generate.
   - Repository access: **Only select repositories** → this repo
   - Permissions → **Contents: Read and write**
4. Open `admin.html`, open "Website connection", paste the token (tick "Remember on this device" on the admin's own phone/computer).
5. Make your QR code point to the customer link.

## Updating the menu (admin)
Open admin.html → choose PDF → Convert → check preview → **Publish to customers**.
The customer link shows the new menu after about 1–2 minutes. The link and QR code never change.

## Security
- Customers can only view. Changing the menu needs the access token.
- Anyone can open admin.html, but without the token they cannot publish.
- If the token is lost or leaked, delete it on GitHub and create a new one.

## Offline
- After a customer opens the menu once with internet, it opens on their phone without internet.
- "Add to Home Screen" gives them a menu icon.
- "Download copy" in admin saves `menu.html` for a tablet or USB stick with no internet at all.
