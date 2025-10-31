# <div align="center">🔐 Fard (فَرْد)</div>

<div align="center">

![Version](https://img.shields.io/badge/version-1.0.0-brightgreen?style=for-the-badge)
![License](https://img.shields.io/badge/license-All_Rights_Reserved-red?style=for-the-badge)
![Security](https://img.shields.io/badge/security-cryptographically_secure-blue?style=for-the-badge)
![Made with Love](https://img.shields.io/badge/made_with-♥-ff69b4?style=for-the-badge)

### *Uniqueness isn't special. It's expected.*

**A cryptographically secure password generator that doesn't compromise.**

[🚀 Live Demo](#) • [📖 Documentation](#features) • [💬 Report Issue](#)

</div>

---

## ✨ What is Fard?

**Fard** (فَرْد) means "unique" or "singular" in Arabic. This password generator lives up to its name by creating truly unique, cryptographically secure passwords using the Web Crypto API. No predictable patterns, no pseudo-random nonsense—just pure randomness powered by your browser's native cryptography.

### 🎯 Philosophy

> In a world where data breaches are common, weak passwords are inexcusable. Fard ensures every password generated is a fortress—unpredictable, strong, and truly random.

---

## 🌟 Features

<table>
<tr>
<td width="50%">

### 🔒 **Cryptographically Secure**
Uses `crypto.getRandomValues()` for true randomness—no Math.random() vulnerabilities here.

### 🎨 **Beautiful Dark/Light Themes**
Switch seamlessly between elegant dark and light modes with smooth transitions.

### 🧩 **Custom Phrase Integration**
Include memorable words or phrases while maintaining security with random character padding.

</td>
<td width="50%">

### ⚙️ **Flexible Configuration**
- Password length: 4-128 characters
- Uppercase, lowercase, numbers, symbols
- Character exclusion options
- Smart placement controls

### 📊 **Real-time Strength Analysis**
Instant entropy calculation and visual strength indicators.

### 🎲 **Smart Generation**
Guarantees at least one character from each selected type.

</td>
</tr>
</table>

---

## 🚀 Getting Started

### Quick Start

1. **Clone the repository:**
   ```bash
   git clone https://github.com/mehedyk/fard.git
   cd fard
   ```

2. **Open `index.html` in your browser:**
   ```bash
   # On macOS
   open index.html
   
   # On Linux
   xdg-open index.html
   
   # On Windows
   start index.html
   ```

3. **Generate passwords immediately!** No build process, no dependencies, no hassle.

### 📦 Or Download

Simply download `index.html` and run it locally. Everything is self-contained in a single file.

---

## 🎮 Usage

### Basic Password Generation

1. **Adjust length** using the slider (4-128 characters)
2. **Select character types** (uppercase, lowercase, numbers, symbols)
3. **Click "Generate Password"** 🎲
4. **Copy with one click** 📋

### Advanced Features

#### 🔤 Include Custom Phrases

Add memorable words or phrases that will be preserved in your password:

```
Phrase: "MyDog2024"
Result: aB7#MyDog2024xK9@pL
```

**Placement Options:**
- **Random** - Phrase appears anywhere in the password
- **Beginning/End** - Randomly chooses start or end position
- **Always Beginning** - Phrase always starts the password
- **Always End** - Phrase always ends the password

#### 🚫 Exclude Ambiguous Characters

Avoid confusing characters like `0O1lI`:

```
Exclude: 0O1lI
Generated: aBcDeFgHjKmNpQrStUvWxYz
```

---

## 🛡️ Security Features

### Cryptographic Randomness

Fard uses the Web Crypto API (`crypto.getRandomValues()`), which provides:

- **True randomness** from the operating system's entropy sources
- **No predictable patterns** unlike `Math.random()`
- **CSPRNG** (Cryptographically Secure Pseudo-Random Number Generator)

### Password Strength Calculation

Each password is analyzed for:
- **Length** (longer = stronger)
- **Character diversity** (uppercase, lowercase, numbers, symbols)
- **Entropy bits** (calculated as: `length × log₂(charset_size)`)

**Strength Ratings:**
- 🔴 **Weak** (score ≤ 3)
- 🟡 **Fair** (score 4-5)
- 🔵 **Good** (score 6-7)
- 🟢 **Very Strong** (score ≥ 8)

### No Data Collection

- ✅ **100% client-side** - passwords never leave your browser
- ✅ **No analytics** - zero tracking or telemetry
- ✅ **No external requests** - works completely offline
- ✅ **Privacy first** - your secrets stay secret

---

## 🎨 Screenshots

<div align="center">

### Dark Mode
![Dark Mode Preview - Elegant green-themed interface with neon accents]

### Light Mode
![Light Mode Preview - Clean, professional interface with forest green palette]

*Seamless theme switching with preserved user preferences*

</div>

---

## 🔧 Technical Details

### Built With

- **Pure HTML/CSS/JavaScript** - No frameworks, no bloat
- **Web Crypto API** - Industry-standard cryptography
- **JetBrains Mono Font** - Beautiful monospace typography
- **CSS Custom Properties** - Dynamic theming system

### Browser Compatibility

| Browser | Minimum Version | Status |
|---------|----------------|--------|
| Chrome | 11+ | ✅ Fully Supported |
| Firefox | 4+ | ✅ Fully Supported |
| Safari | 3.1+ | ✅ Fully Supported |
| Edge | 12+ | ✅ Fully Supported |
| Opera | 15+ | ✅ Fully Supported |

### File Structure

```
fard/
├── index.html          # Complete application (self-contained)
├── README.md          # This file
└── LICENSE            # License information
```

---

## 💡 Why Fard?

### vs. Other Password Generators

| Feature | Fard | Others |
|---------|------|--------|
| Cryptographically Secure | ✅ | ⚠️ Some use Math.random() |
| Offline Capable | ✅ | ❌ Often require internet |
| Custom Phrase Integration | ✅ | ❌ Rare feature |
| Theme Support | ✅ | ⚠️ Limited |
| Single File | ✅ | ❌ Usually multi-file |
| Privacy Focused | ✅ | ⚠️ Varies |
| Open Inspection | ✅ | ⚠️ Often obfuscated |

### Use Cases

- 🏢 **Enterprise** - Generate secure credentials for systems
- 👤 **Personal** - Create strong passwords for online accounts
- 🔐 **Security Audits** - Test password strength requirements
- 📚 **Education** - Teach password security principles
- 🛠️ **Development** - Generate API keys, tokens, secrets

---

## 📋 Roadmap

- [ ] Password history with secure storage
- [ ] Bulk password generation
- [ ] Custom symbol sets
- [ ] Passphrase generator mode
- [ ] Password strength requirements checker
- [ ] Export passwords to encrypted file

---

## 🤝 Contributing

### 🚨 IMPORTANT: Read License First

**Fard is proprietary software.** Before contributing:

1. Read the [LICENSE](#-license) section carefully
2. Understand that all contributions become proprietary
3. Contact [@mehedyk](https://github.com/mehedyk) for permission

### How to Contribute (If Approved)

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📜 License

```
Copyright (c) 2024 @mehedyk (https://github.com/mehedyk)
All Rights Reserved.

PROPRIETARY LICENSE

This software and associated documentation files (the "Software") are the 
exclusive property of @mehedyk. 

TERMS AND CONDITIONS:

1. RESTRICTIONS
   ❌ NO reproduction, modification, or distribution
   ❌ NO creation of derivative works
   ❌ NO reverse engineering or decompilation
   ❌ NO commercial or non-commercial use without written permission
   ❌ NO public hosting without explicit authorization
   ❌ NO removal or alteration of copyright notices

2. PERMITTED USES
   ✅ Personal inspection of source code for security review
   ✅ Running the software locally for personal password generation
   ✅ Reporting security vulnerabilities to the author

3. ATTRIBUTION
   Any permitted use must maintain all copyright notices and attribution
   to @mehedyk (https://github.com/mehedyk).

4. NO WARRANTY
   THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
   OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
   FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.

5. LIABILITY
   IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
   LIABILITY ARISING FROM THE USE OF THE SOFTWARE.

6. PERMISSION REQUESTS
   For licensing inquiries, commercial use, or permission requests:
   Contact: https://github.com/mehedyk

VIOLATION OF THESE TERMS CONSTITUTES COPYRIGHT INFRINGEMENT AND MAY RESULT
IN LEGAL ACTION.
```

### 🔴 License Summary (Non-Legal)

**You MAY:**
- ✅ Use Fard locally for personal password generation
- ✅ Inspect the code to verify security claims
- ✅ Report bugs and vulnerabilities

**You MAY NOT:**
- ❌ Copy, modify, or redistribute the code
- ❌ Use the code in your own projects
- ❌ Host Fard publicly without permission
- ❌ Remove the author's credits
- ❌ Create derivative works

**Want to use Fard commercially?** Contact [@mehedyk](https://github.com/mehedyk) for licensing options.

---

## 🐛 Bug Reports & Security

### Found a Bug?

Please report issues with:
- **Description** - What happened?
- **Steps to reproduce** - How can we see it?
- **Expected behavior** - What should happen?
- **Browser & OS** - Your environment details

### 🔒 Security Vulnerabilities

If you discover a security issue:

1. **DO NOT** open a public issue
2. **Email** security details privately to [@mehedyk](https://github.com/mehedyk)
3. Include detailed reproduction steps
4. Allow reasonable time for a fix before disclosure

---

## 👨‍💻 Author

<div align="center">

<img src="https://github.com/mehedyk.png" width="150" height="150" style="border-radius: 50%; border: 4px solid #39ff14;" alt="mehedyk">

### **S.M. Mehedy Kawser**
### [@mehedyk](https://github.com/mehedyk)

<!--- *Software Developer • Security Enthusiast • Open Source Advocate* -->

[![GitHub](https://img.shields.io/badge/GitHub-mehedyk-181717?style=for-the-badge&logo=github)](https://github.com/mehedyk)
[![Portfolio](https://img.shields.io/badge/Portfolio-Visit-39ff14?style=for-the-badge&logo=web)](https://github.com/mehedyk)

</div>

---

**About the Author:**

Passionate about creating secure, privacy-focused tools that respect users. Fard represents a commitment to making strong security accessible to everyone without compromising on design or usability.

> "Security shouldn't be an afterthought, and good design shouldn't sacrifice functionality."

---

## 📞 Contact & Support

<div align="center">

**Questions? Licensing inquiries? Feature requests?**

[Open an Issue](https://github.com/mehedyk/fard/issues) • [Visit Profile](https://github.com/mehedyk) • [Email](mailto:kawser2305341202@diu.edu.bd)

### Get in Touch

- 💼 **Professional Inquiries:** [GitHub Profile](https://github.com/mehedyk)
- 🐛 **Bug Reports:** [Issue Tracker](https://github.com/mehedyk/fard/issues)
- 🔒 **Security:** Private disclosure to [@mehedyk](https://github.com/mehedyk)
- 📜 **Licensing:** Contact for commercial use permissions

</div>

---

## ⭐ Show Your Support

If you find Fard useful:

- ⭐ **Star this repository** to show appreciation
- 🐦 **Share** with others who need secure passwords
- 💬 **Provide feedback** to help improve the tool

---

<div align="center">

### 🔐 Stay Secure. Stay Unique. Stay Fard.

**Made by [@mehedyk](https://github.com/mehedyk)**

*Fard (فَرْد) - Because your security deserves uniqueness.*

---

![Footer Banner](https://img.shields.io/badge/🔐-Cryptographically_Secure-brightgreen?style=for-the-badge)
![Footer Banner](https://img.shields.io/badge/🎨-Beautiful_Design-blue?style=for-the-badge)
![Footer Banner](https://img.shields.io/badge/🚀-Zero_Dependencies-orange?style=for-the-badge)

</div>