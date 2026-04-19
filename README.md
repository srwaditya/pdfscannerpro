# 🔒 DocScanner Pro — Privacy Policy

This folder contains the privacy policy page for the **DocScanner Pro** Android app (Document Scanner & PDF Creator).

## 📁 Files

| File | Description |
|------|-------------|
| `index.html` | The privacy policy web page (dark themed, mobile-friendly) |
| `README.md` | This file |

---

## 🚀 How to Host on GitHub Pages

Follow these steps to get a live URL for your Play Store listing:

### Step 1 — Create a GitHub Repository
1. Go to [github.com/new](https://github.com/pdfscannerpro

2. Repository name: `docscanner-privacy`
3. Set it to **Public**
4. ❌ Do **not** check "Add a README"
5. Click **Create repository**

### Step 2 — Push the Files
Run these commands from the `privacy_policy` folder:
```bash
cd "/Users/srw.aditya/Downloads/pdf scaneer/privacy_policy"
git remote add origin https://github.com/srwaditya/docscanner-privacy.git
git push -u origin main
```

### Step 3 — Enable GitHub Pages
1. Go to your repo → **Settings** tab
2. Scroll to **Pages** in the left sidebar
3. Under **Source**, select `main` branch and `/ (root)` folder
4. Click **Save**

### Step 4 — Get Your URL
After ~1 minute, your privacy policy will be live at:
```
https://srwaditya.github.io/docscanner-privacy/
```

---

## 📱 Use in Play Store

Paste your GitHub Pages URL in:

> **Google Play Console → App Content → Privacy Policy → Save**

---

## 📋 What the Policy Covers

The privacy policy addresses all permissions used by DocScanner Pro:

| Permission | Covered |
|------------|---------|
| `android.permission.CAMERA` | ✅ Yes |
| `android.permission.READ_EXTERNAL_STORAGE` | ✅ Yes |
| `android.permission.WRITE_EXTERNAL_STORAGE` | ✅ Yes |
| `android.permission.READ_MEDIA_IMAGES` | ✅ Yes |
| `android.permission.INTERNET` (AdMob) | ✅ Yes |
| `android.permission.ACCESS_NETWORK_STATE` | ✅ Yes |

---

## 📲 Add to App (Optional)

You can add a **"Privacy Policy"** button in your Flutter app's settings screen using `url_launcher`:

```dart
import 'package:url_launcher/url_launcher.dart';

const privacyUrl = 'https://srwaditya.github.io/docscanner-privacy/';

Future<void> openPrivacyPolicy() async {
  final uri = Uri.parse(privacyUrl);
  if (await canLaunchUrl(uri)) {
    await launchUrl(uri, mode: LaunchMode.externalApplication);
  }
}
```

---

## 📬 Contact

Developer: **Aditya Shrivastava**  
Email: srw.aditya@gmail.com
