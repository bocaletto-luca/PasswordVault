# Password Generator & Vault

A modern, responsive, single-page password manager and generator.  
Generate strong passwords in-browser, encrypt and store them locally with username/email, filter, import/export JSON, copy to clipboard—no server or external libraries required.

---

## 🔗 Live Demo

https://bocaletto-luca.github.io/PasswordVault/index.html

---

## 🚀 Features

- **Secure Password Generator**  
  • Include lowercase, UPPERCASE, numbers, symbols  
  • Customizable length (4–64 characters)  
  • One-click copy to clipboard  

- **Encrypted Vault**  
  • AES-GCM encryption with PBKDF2 key-derivation  
  • Master password protects all entries  
  • Data stored in `localStorage` (no server)  

- **Entry Management**  
  • Save site/app, username/email, and password  
  • Inline edit or delete any entry  
  • Reveal password on focus, hide on blur  
  • Copy individual passwords with one click  

- **Filtering & Search**  
  • Live filter by site/app or username/email  
  • Instant results in table view  

- **Import / Export JSON**  
  • Export entire vault as encrypted JSON  
  • Import vault JSON backup or migrate between devices  

- **Print-Ready & SEO Optimized**  
  • Print view hides UI controls  
  • Semantic HTML, meta tags, and JSON-LD schema  

---

## 🛠️ Getting Started

### Prerequisites

- Modern web browser (Chrome, Firefox, Safari, Edge)

### Installation

1. **Clone the repository**  
   ```bash
   git clone https://github.com/bocaletto-luca/PasswordVault.git
   ```
2. **Open the app**  
   - Navigate into the project folder  
   - Open `index.html` in your browser  

No build or install steps required.

---

## 🎯 Usage

### 1. Generator Tab

1. Select character sets (lowercase, UPPERCASE, numbers, symbols)  
2. Set desired length (4–64)  
3. Click **Generate**  
4. Copy the generated password or paste it into the vault form

### 2. Vault Tab

1. Click **Vault** to switch tabs  
2. **First use:** set your Master Password  
3. **Subsequent uses:** enter Master Password to unlock  
4. Add a new entry:
   - Site / App  
   - Username / Email  
   - Password (paste or generate)  
   - Click **Save Entry**

5. Manage entries:
   - **Edit** inline fields; changes auto-save  
   - **Reveal** password by focusing the field  
   - **Copy** password to clipboard  
   - **Delete** entry with confirmation  

6. **Filter** entries by site or user using the search box

### 3. Import / Export

- **Export JSON**: download encrypted vault data  
- **Import JSON**: upload a previously exported file (Vault will relock; unlock again to view)

### 4. Print

Click **Print Quiz** (in modal) to view print-friendly layout with controls hidden.

---

## 🔒 Encryption & Security

- **Master Password**: chosen by you; not stored in plain text  
- **Key Derivation**: PBKDF2 with 100,000 iterations & SHA-256  
- **Encryption**: AES-GCM 256-bit  
- **Salt & IV**: randomly generated, stored in `localStorage`  

> **Warning:** If you forget your Master Password, vault data cannot be recovered. Deleting keys and vault data resets the app.

---

## 🧰 Built With

- HTML5 & CSS3 (Grid, Flexbox, Custom Properties)  
- Vanilla JavaScript (ES6+)  
- Web Crypto API for encryption  
- `localStorage` for persistence  

---

## 🤝 Contributing

Contributions are welcome!

1. Fork the repo  
2. Create a feature branch  
   ```bash
   git checkout -b feature/YourFeature
   ```
3. Commit your changes  
   ```bash
   git commit -m "Add awesome feature"
   ```
4. Push to your fork  
   ```bash
   git push origin feature/YourFeature
   ```
5. Open a Pull Request

---

## 📄 License

This project is licensed under the [GPL-3.0 License](https://www.gnu.org/licenses/gpl-3.0.en.html).

---

## 👤 Author

**Bocaletto Luca**  
- GitHub: [@bocaletto-luca](https://github.com/bocaletto-luca)  
- Live Demo: https://bocaletto-luca.github.io/PasswordVault/index.html
