# ESP32 Counter Dashboard

This repository contains a mobile-friendly dashboard for viewing an ESP32 pulse counter.

## How to Deploy to GitHub Pages

1. Upload `index.html` to your GitHub repository.
2. Go to **Settings → Pages**
3. Set:
   - Source: Deploy from branch
   - Branch: main
   - Folder: root
4. Save
5. Your site will publish at:
   `https://YOUR-USERNAME.github.io/REPO-NAME/`

## ESP32 Endpoint
The dashboard expects the ESP32 to provide JSON at:

`http://192.168.1.50/data`

Example JSON format:

```
{
  "count": 123,
  "hourTotals": [5, 9, 22, ...]
}
```

Change the IP in the script if needed.
