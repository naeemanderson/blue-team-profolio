# 📨 TryHackMe: Phishing Emails 1

This lab focuses on analyzing suspicious emails using tools like **Thunderbird**, **CyberChef**, and **Linux CLI**.

## 🛠️ Tools Used
- Thunderbird
- CyberChef
- Linux command line
- URL analysis tools

## 🔍 Key Skills Practiced
- Raw email header inspection
- Base64 decoding of attachments
- PDF reconstruction
- URI verification

  ### ✅ Header Analysis
- Reviewed `Return-Path`, `From`, and `Received` fields to track email origin.
- Used email client tools to inspect hidden headers.

### ✅ Attachment Reconstruction
- Found embedded base64-encoded payloads (PDF).
- Used CyberChef to remove whitespace and decode base64.
- Saved and safely opened reconstructed PDFs to assess content.

### ✅ Link/URI Verification
- Detected and validated blocked image URIs like:
https://i.imgur.com/LSWOtDI.png

yaml
Copy
Edit
- Compared link display text with actual redirect targets (classic phishing indicator).

### ✅ Phishing Indicators Identified
- Mismatched sender domain vs. display name
- Use of urgency ("click now", "document required")
- Unusual sending times and obfuscated links

---

## ✍️ Final Thoughts

This room was a hands-on introduction to email forensics. It sharpened my awareness of how real-world phishing attempts hide in plain sight and emphasized the value of inspecting raw email data, not just the UI layer.

---
