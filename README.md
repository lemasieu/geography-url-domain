# Geography URL Domain

A simple, interactive web tool that extracts the top-level domain (TLD) from a URL and identifies the associated geographical location (country, city, or continent).

## 🚀 Live Demo

Check out the live demo: [https://www.xn--msiu-goa8b.vn/github/geography-url-domain](https://www.xn--msiu-goa8b.vn/github/geography-url-domain)

## ✨ Features

- **Extract TLD** – Automatically extracts the top-level domain from any valid URL
- **Identify Location** – Matches the TLD against a comprehensive database to find the associated country, city, or continent
- **Supports Multiple TLD Types** – Handles country-code TLDs (e.g., .vn, .us), generic TLDs (e.g., .asia, .africa), and city TLDs (e.g., .paris, .tokyo)
- **Real-Time Results** – Displays the extracted domain and its geographical location instantly
- **Clean Interface** – Simple, user-friendly design with a clear layout
- **Responsive** – Works on desktop, tablet, and mobile devices

## 🛠️ Technologies Used

- HTML5
- CSS3
- JavaScript (Vanilla)
- JSON (geographical domain data)

## 📁 Project Structure

```
geography-url-domain/
├── index.html        # Main HTML file
├── style.css         # Stylesheet
├── script.js         # JavaScript logic for domain extraction and lookup
├── data.json         # Geographical domain data (countries, cities, continents)
└── README.md         # Project documentation
```


## 🔧 Installation & Usage

1. **Clone the repository**
   ```bash
   git clone https://github.com/lemasieu/geography-url-domain.git
   ```
2. **Navigate to the project folder**
   ```bash
   cd geography-url-domain
   ```
   
3. **Run the application with a local server**

⚠️ Important: This project loads data from a JSON file, so you need to use a local development server instead of opening `index.html` directly in your browser to avoid CORS issues.

- **Using VS Code** – Install the "Live Server" extension, right-click on `index.html`, and select "Open with Live Server"
- **Using Python** – Run `python -m http.server` (Python 3) or `python -m SimpleHTTPServer` (Python 2) and open `http://localhost:8000`
- **Using Node.js** – Install `http-server` globally (`npm install -g http-server`) and run `http-server` in the project folder

## 📝 How It Works

1. **Enter a URL** – Type any valid URL (e.g., `https://example.com`, `example.co.uk`, or `site.paris`) into the input field
2. **Click "Tìm kiếm" (Search)** – The tool processes the URL and extracts the top-level domain
3. **View the results** – The first output field shows the extracted domain, and the second shows the associated geographical location

### How domains are processed:

The tool extracts the top-level domain (TLD) from the URL and searches the data.json database in the following order:

1. **Country TLDs** – Matches against country-code top-level domains (e.g., `.vn` → Vietnam, `.fr` → France)
2. **City TLDs** – Matches against geographic/city top-level domains (e.g., `.paris` → Paris, France, `.tokyo` → Tokyo, Japan)
3. **Continent TLDs** – Matches against continental top-level domains (e.g., `.asia` → Asia, `.africa` → Africa)

### Supported Location Types:

- **Countries** – Over 200 country TLDs including internationalized domain names (e.g., `.中国` for China, `.日本` for Japan)
- **Cities** – Major cities worldwide including Cape Town, Dubai, Paris, Tokyo, London, and many more
- **Continents** – Africa, Asia, Arab, and Latin America

## 🤝 Contributing

Contributions are welcome! Feel free to submit a Pull Request or open an Issue.
1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is open-source and available under the MIT License.
