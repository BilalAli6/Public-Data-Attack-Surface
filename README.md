# 🌐 From OSINT to Exploitation: How Public Data Becomes an Attack Surface

## 🎤 Context
This repository supports my talk submission to Positive Hack Talks Kuala Lumpur 2026.

It demonstrates how publicly available data and user interactions can be leveraged to build an attack surface — without exploiting real systems.

---

## ⚠️ Disclaimer
This project is strictly for educational and defensive purposes.

- All demonstrations were performed in a controlled lab environment  
- No real users or systems were targeted  
- Sensitive data has been intentionally excluded  

---

# ⚙️ Setup

## 🛠️ Install ExifTool
```bash
sudo apt update
sudo apt install exiftool
````

## 🛠️ Install Social-Engineer Toolkit (SET)

```bash
sudo apt install set
sudo setoolkit
```

---

# 📸 STEP 1 — Metadata Extraction (ExifTool)

## 🎯 Objective

Extract hidden information from images.

## 💻 Commands

```bash
exiftool me.png
exiftool eastwood.jpeg
```

## 🧾 Output

### me.png

```
File Type : PNG
Image Width : 460
Image Height : 460
Bit Depth : 8
Color Type : RGB
```

### eastwood.jpeg

```
File Type : JPEG
Image Width : 183
Image Height : 275
Encoding Process : Baseline DCT
```

## 📷 Screenshots
<img width="940" height="528" alt="image" src="https://github.com/user-attachments/assets/cca47534-2494-434a-918d-191f6ce6ef0d" />

<img width="940" height="528" alt="image" src="https://github.com/user-attachments/assets/0a1bd451-003c-4822-be7e-9a7d3f4e5e2e" />

<img width="940" height="528" alt="image" src="https://github.com/user-attachments/assets/29e4987b-f303-4506-87c9-223db499eaf9" />
<img width="940" height="528" alt="image" src="https://github.com/user-attachments/assets/d117fd69-a2e3-4ba9-b5f0-1a6f76f651a8" />



## 💡 Insight

Even simple images can contain hidden metadata.
In real-world cases, this may expose:

* Location
* Device information
* Timestamps

---

# 🔑 STEP 2 — Data Breach Analysis

## 🎯 Objective

Check whether an email has been exposed in public breaches.

## 🌐 Tool

* Have I Been Pwned → [https://haveibeenpwned.com](https://haveibeenpwned.com)

## 📌 Steps

1. Visit: [https://haveibeenpwned.com](https://haveibeenpwned.com)
2. Enter a test email (self-owned/dummy)
3. Review breach results

## 📷 Screenshots

<img width="940" height="434" alt="image" src="https://github.com/user-attachments/assets/e7a675f2-e4a4-49e2-be02-d3c1f45bf037" />

<img width="940" height="432" alt="image" src="https://github.com/user-attachments/assets/018827e4-f9c8-4961-be36-5432438b190a" />



## 💡 Insight

A single breach can expose:

* Emails
* Passwords
* Usernames

Credential reuse significantly increases risk.

---

# 🎭 STEP 3 — Social Engineering Simulation (SET)

## 🎯 Objective

Demonstrate how attackers can intercept user input using cloned interfaces.

## 💻 Process

1. Run:

```bash
sudo setoolkit
```

2. Navigate:

```
1) Social-Engineering Attacks
2) Website Attack Vectors
3) Credential Harvester Attack Method
1) Web Templates
```

3. Select template (e.g., Google)
4. Use localhost (127.0.0.1) for safe testing

---

## 🧾 Output (Sanitized)

```
[*] Credential Harvester is running
[*] WE GOT A HIT!
PARAM: service=login
PARAM: continue=...
```

## 📷 Screenshots

<img width="940" height="438" alt="image" src="https://github.com/user-attachments/assets/e5a790d3-4880-4010-8986-02b6f02fadd9" />
<img width="940" height="437" alt="image" src="https://github.com/user-attachments/assets/47871c96-c7aa-4dbb-8472-52eff0aa4347" />
<img width="940" height="441" alt="image" src="https://github.com/user-attachments/assets/70892e96-3e05-4c05-97e7-a2c900a75b10" /><img width="940" height="441" alt="image" src="https://github.com/user-attachments/assets/bf7ef9cb-7014-4c1d-bfdb-54e9d640c873" />
<img width="940" height="462" alt="image" src="https://github.com/user-attachments/assets/637999bc-c0c3-48a9-9e23-2a517db93b88" />
<img width="940" height="439" alt="image" src="https://github.com/user-attachments/assets/644327f5-585b-45c7-bb6b-601f0b336f6f" />







## 💡 Insight

This attack relies on **user trust**, not system vulnerabilities.

⚠️ Sensitive fields (username/password) have been intentionally removed.

---

# 🛡️ Defensive Takeaways

* Verify URLs before login
* Use Multi-Factor Authentication (MFA)
* Avoid password reuse
* Strip metadata before sharing images
* Monitor breach exposure regularly

---

# 📬 Contact & Connect

If you have questions, want to discuss OSINT defensive strategies, or are attending Positive Hack Talks KL 2026, connect here:

* LinkedIn: Muhammad Bilal Ali Saif
* GitHub: BilalAli6
* Email: bilalalisaif6@gmail.com
* Project Repository: [Public Data Attack Surface](https://github.com/BilalAli6/public-data-attack-surface/)

---

# 💎 Acknowledgments
* Social-Engineer Toolkit (SET)
* ExifTool by Phil Harvey
* Have I Been Pwned
* Positive Hack Talks Kuala Lumpur Committee

---

# ⚖️ License
Distributed under the MIT License. See [LICENSE](https://github.com/BilalAli6/public-data-attack-surface/blob/main/LICENSE) for details.

---

# 🧠 Final Message

This demo shows how:

* Small pieces of public data
* Combined with user behavior

can lead to real security risks.

No advanced exploitation required — just **data exposure + human factors**.


