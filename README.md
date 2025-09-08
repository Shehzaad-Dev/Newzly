📰 Newzly – Real-Time News App

A Flutter-based mobile application that delivers real-time breaking news and categorized headlines from trusted global sources. Features a clean, modern interface with smooth navigation and optimized performance.


🚀 Features

· Top Headlines: Curated breaking news from multiple countries.
· Categorized News: Browse by category including Technology, Sports, Business, Health, and Entertainment.
· Search Functionality: Find news articles on any topic.
· Article Previews: View images, titles, publication dates, and sources without leaving the app.
· WebView Integration: Seamlessly open full articles in an in-app browser.
· Theme Support: Built with support for Light and Dark themes.


🛠️ Tech Stack

· Framework: Flutter
· Language: Dart
· API: NewsAPI.org
· HTTP Requests: http package
· State Management: Provider / Bloc (State Management)
· Image Caching: cached_network_image package
· In-App Browser: webview_flutter package


🔧 Installation & Setup

1. Get an API Key:
   · Obtain a free API key from NewsAPI.org.
2. Clone the repository:
   ```bash
   git clone https://github.com/Shehzaad-Dev/Newzly.git
   cd Newzly
   ```
3. Configure API Key:
   · Create a .env file in the root directory.
   · Add your API key: NEWS_API_KEY=your_api_key_here
4. Install dependencies and run:
   ```bash
   flutter pub get
   flutter run
   ```


📁 Project Structure

```
lib/
├── main.dart                    # Application entry point
├── models/                      # Data models (Article, NewsResponse)
├── services/                    # Business logic & API calls
│   └── news_service.dart
├── screens/                     # Full app screens
│   ├── home_screen.dart
│   └── detail_screen.dart
├── widgets/                     # Reusable UI components
│   ├── news_card.dart
│   └── category_list.dart
├── utils/                       # Constants & helpers
│   └── constants.dart
assets/                         # Images, icons, etc.
```


🔒 Security Considerations

This project was developed with a security-first mindset, incorporating practices essential for modern mobile applications:

· API Key Management: The NewsAPI key is stored securely using environment variables (.env) to prevent exposure in version control. This mitigates the risk of unauthorized API usage and quota theft.
· Data Validation: All data fetched from the external API is validated and parsed using Dart's strong type system to prevent malformed data from causing runtime exceptions or unexpected behavior.
· Secure Communication: All network requests are made over HTTPS to ensure end-to-end encryption of news data in transit, protecting against man-in-the-middle (MITM) attacks.
· Input Sanitization: User inputs, particularly in the search functionality, are sanitized to guard against potential injection attacks targeting the app's UI or the underlying WebView.
· Dependency Vigilance: Relied on well-maintained, popular packages from pub.dev and regularly checked for updates to avoid incorporating libraries with known vulnerabilities.

Building Newzly provided hands-on experience in integrating third-party APIs securely and understanding the OWASP Mobile Application Security (MAS) guidelines.


👨‍💻 Developer

Muhammad Shehzad
Security-Focused Flutter Developer | AppSec Enthusiast

· 📧 Email: shehzadwazir911@gmail.com
· 💼 LinkedIn: muhammadshehzad-dev
· 🐙 GitHub: Shehzaad-Dev

Open to: Cybersecurity & Application Security Internships


⭐ If you find this project useful, please give it a star on GitHub!