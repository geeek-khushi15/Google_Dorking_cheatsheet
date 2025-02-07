# Google Dorking Cheat Sheet

Google Dorking helps in performing advanced searches using Google operators to find specific information.

## 🔍 Basic Operators

| Operator   | Description                                      | Example |
|------------|--------------------------------------------------|---------|
| `site:`    | Search within a specific site                   | `site:example.com` |
| `inurl:`   | Find URLs containing a keyword                  | `inurl:login` |
| `intitle:` | Find pages with a keyword in the title          | `intitle:index of` |
| `allintitle:` | All words must be in the title               | `allintitle:admin login` |
| `intext:`  | Search for a word in page text                  | `intext:password` |
| `allintext:` | All words must be in page text               | `allintext:confidential file` |
| `filetype:`| Search for a specific file type                 | `filetype:pdf cybersecurity` |
| `ext:`     | Same as filetype:                               | `ext:xls site:example.com` |
| `cache:`   | View Google’s cached version of a page         | `cache:example.com` |
| `related:` | Find similar websites                          | `related:example.com` |
| `link:`    | Find sites linking to a URL                    | `link:example.com` |

## 🔥 Advanced Dorks for Finding Sensitive Information

| Dork  | Purpose |
|-------|---------|
| `inurl:wp-admin` | Find WordPress admin pages |
| `inurl:php?id=` | Identify vulnerable SQL injection pages |
| `intitle:"index of" "parent directory"` | Find directory listings |
| `filetype:sql intext:"INSERT INTO"` | Find exposed SQL databases |
| `filetype:log intext:"password"` | Find log files containing passwords |
| `site:pastebin.com intext:"password"` | Find leaked credentials on Pastebin |
| `site:drive.google.com intext:"confidential"` | Search for confidential Google Drive files |

## 🎥 Finding Cameras & IoT Devices

| Dork  | Purpose |
|-------|---------|
| `inurl:"viewerframe?mode="` | Open camera feeds |
| `inurl:"top.htm" intext:"Live View / - AXIS"` | Axis camera feeds |
| `inurl:"control/userimage.html"` | Vulnerable webcam panels |

## 🛡 Finding Admin Portals

| Dork  | Purpose |
|-------|---------|
| `intitle:"admin login"` | Find admin login pages |
| `inurl:admin/login` | Search for admin panels |
| `inurl:dashboard filetype:php` | Search for web dashboards |

## 📄 Finding Sensitive Documents

| Dork  | Purpose |
|-------|---------|
| `filetype:pdf intext:"confidential"` | Find confidential PDFs |
| `filetype:xls intext:"username password"` | Find Excel files with login details |
| `filetype:docx intext:"internal use only"` | Find restricted documents |

## 📧 Finding Email Lists

| Dork  | Purpose |
|-------|---------|
| `intext:"@gmail.com" filetype:xls` | Find email lists in Excel files |
| `intext:"@yahoo.com" filetype:csv` | Find email lists in CSV files |

## 🔑 Miscellaneous Useful Dorks

| Dork  | Purpose |
|-------|---------|
| `site:github.com "DB_PASSWORD"` | Find database passwords on GitHub |
| `site:pastebin.com "API_KEY"` | Search for API keys on Pastebin |
| `inurl:wp-content/uploads` | Find WordPress uploads |

---

⚠ **Disclaimer:** This cheat sheet is for **educational purposes only**. Unauthorized access to sensitive data is **illegal**.
