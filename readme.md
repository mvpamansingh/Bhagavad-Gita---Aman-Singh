# 🕉️ Bhagavad Gita - Krishn Bhakti

<p align="center">
  <img src="https://img.shields.io/badge/Android-35+-brightgreen" alt="Android API Level">
  <img src="https://img.shields.io/badge/Kotlin-1.9.0+-purple" alt="Kotlin Version">
  <img src="https://img.shields.io/badge/Jetpack%20Compose-Latest-blue" alt="Jetpack Compose">
  <img src="https://img.shields.io/badge/Material%203-Yes-orange" alt="Material 3">
</p>

<p align="center">
A beautiful, feature-rich Android application that brings the timeless wisdom of the Bhagavad Gita to your mobile device. Experience the sacred teachings of Lord Krishna with modern UI design and comprehensive spiritual content.
</p>

## 📱 Screenshots

<!-- Add your app screenshots here -->

## ✨ Features

### 🏠 **Home Screen**
- **Verse of the Day**: Start each day with divine inspiration
- **Last Read Tracking**: Continue your spiritual journey from where you left off
- **Beautiful Sanskrit Typography**: Authentic display of Sanskrit verses
- **Quick Navigation**: Easy access to all app features

### 📖 **Sacred Text Features**
- **Complete Bhagavad Gita**: All 18 chapters with 700 verses
- **Multiple Translations**: English translations from renowned scholars
- **Sanskrit Text**: Original Sanskrit verses with transliteration
- **Commentary**: Detailed explanations and interpretations
- **Word Meanings**: Understand each Sanskrit word's significance

### 🔖 **Bookmarking System**
- **Save Chapters**: Bookmark entire chapters for easy access
- **Verse Bookmarks**: Mark individual verses for reference
- **Personal Library**: Organize your saved spiritual content
- **Quick Access**: Navigate directly to bookmarked content

### 🏛️ **Virtual Temple**
- **Sacred Experience**: Create a divine atmosphere for meditation
- **Interactive Elements**: Immersive spiritual environment
- **Peaceful Interface**: Designed for contemplation and prayer

### 📚 **Krishna Leela Stories**
- **Divine Pastimes**: Explore stories from Krishna's life
- **Chapter Organization**: Well-structured narrative content
- **Rich Storytelling**: Engaging presentation of sacred tales
- **Spiritual Wisdom**: Learn through divine stories

### 🎵 **Krishna Mantras**
- **Sacred Chants**: Collection of powerful mantras
- **Devotional Practice**: Support for daily spiritual routine
- **Audio Integration**: (Feature in development)

### 🎨 **Customization & Themes**
- **Multiple Themes**: Choose from various spiritual color schemes
- **Dark/Light Mode**: Comfortable reading in any environment
- **Font Options**: Optimized typography for Sanskrit and English
- **Personalized Experience**: Customize based on your preferences

### ⚙️ **Settings & Profile**
- **User Profile**: Personalize your spiritual journey
- **Reading Preferences**: Customize your reading experience
- **About Developer**: Learn about the app creator
- **App Information**: Version details and acknowledgments

## 🛠️ Tech Stack

### **Frontend & UI**
- **[Kotlin](https://kotlinlang.org/)** - Modern, concise programming language
- **[Jetpack Compose](https://developer.android.com/jetpack/compose)** - Modern Android UI toolkit
- **[Material 3 Design](https://m3.material.io/)** - Latest Material Design system
- **[Navigation Compose](https://developer.android.com/jetpack/compose/navigation)** - Type-safe navigation

### **Architecture & Patterns**
- **MVVM (Model-View-ViewModel)** - Clean architecture pattern
- **Repository Pattern** - Data access abstraction
- **Use Cases** - Business logic encapsulation
- **State Management** - Compose state and ViewModels

### **Database & Storage**
- **[Room Database](https://developer.android.com/training/data-storage/room)** - Local SQLite database
- **[DataStore](https://developer.android.com/topic/libraries/architecture/datastore)** - Preferences and settings storage
- **Type Converters** - Complex data serialization

### **Networking & Data**
- **[Retrofit](https://square.github.io/retrofit/)** - REST API client
- **[OkHttp](https://square.github.io/okhttp/)** - HTTP client with logging
- **[Gson](https://github.com/google/gson)** - JSON serialization
- **[Kotlin Serialization](https://kotlinlang.org/docs/serialization.html)** - Native Kotlin serialization

### **Dependency Injection**
- **[Koin](https://insert-koin.io/)** - Lightweight dependency injection framework
- **Modular DI** - Organized dependency modules

### **Media & Animations**
- **[Coil](https://coil-kt.github.io/coil/)** - Image loading library with Compose support
- **[Lottie](https://lottiefiles.com/)** - Vector animations
- **SVG Support** - Scalable vector graphics

### **Development Tools**
- **Kotlin Parcelize** - Parcelable implementation
- **Kapt** - Annotation processing
- **ProGuard** - Code obfuscation and optimization

## 🏗️ Project Structure

```
app/src/main/java/com/mvpamansingh/shrimadbhagavadgita/
├── data/
│   ├── di/                     # Dependency injection modules
│   ├── local/                  # Room database, DAOs, entities
│   └── remote/                 # API services and networking
├── domain/
│   ├── models/                 # Data models and entities
│   ├── repository/             # Repository interfaces and implementations
│   └── datastore/             # DataStore preferences
├── presentation/
│   ├── allChapters/           # Chapters listing screen
│   ├── chapterDetailWithVerses/ # Chapter verses screen
│   ├── verseDetailsScreen/    # Individual verse details
│   ├── bookMarkScreen/        # Bookmarks management
│   ├── homeScreen/            # Main home screen
│   ├── virtualTempleScreen/   # Virtual temple experience
│   ├── CategoryScreen/        # Krishna Leela & Mantras
│   ├── settingScreen/         # Settings and profile
│   ├── splashScreen/          # Onboarding screens
│   ├── common/                # Reusable UI components
│   └── navigation/            # Navigation graphs and routes
└── ui/theme/                  # Theme, colors, and typography
```

## 🚀 Getting Started

### Prerequisites
- **Android Studio** - Arctic Fox or later
- **Android SDK** - API level 24 or higher
- **JDK** - Version 11 or higher

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/BhagavadGitaGyan.git
   cd BhagavadGitaGyan
   ```

2. **Open in Android Studio**
   - Launch Android Studio
   - Select "Open an existing project"
   - Navigate to the cloned repository
   - Wait for Gradle sync to complete

3. **Build and Run**
   ```bash
   ./gradlew clean build
   ./gradlew installDebug
   ```

### Configuration

1. **API Configuration** (if applicable)
   - Add your API keys to `local.properties`
   - Configure network endpoints in `GeetaApi.kt`

2. **Database Setup**
   - Room database is automatically initialized
   - No manual setup required for local storage

## 📖 API Integration

The app integrates with Bhagavad Gita APIs to fetch:
- Chapter information and summaries
- Verse details with translations
- Commentary from various authors
- Sanskrit text and transliterations

### Data Models
```kotlin
data class VerseDetail(
    val chapter_number: Int,
    val verse_number: Int,
    val text: String,                    // Sanskrit verse
    val transliteration: String,         // Roman transliteration
    val word_meanings: String,           // Word-by-word meaning
    val translations: List<Translation>, // Multiple translations
    val commentaries: List<Commentary>   // Scholarly commentary
)
```

## 🎨 UI/UX Features

### **Design Philosophy**
- **Spiritual Aesthetics** - Colors and fonts inspired by traditional Indian art
- **Sacred Typography** - Authentic Sanskrit fonts and proper diacritics
- **Peaceful Interface** - Calming colors and smooth animations
- **Accessibility** - Support for different text sizes and contrast

### **Interactive Elements**
- **Smooth Navigation** - Custom transitions between screens
- **Lottie Animations** - Engaging micro-interactions
- **Material 3 Components** - Modern, familiar UI patterns
- **Responsive Design** - Optimized for different screen sizes

## 🔧 Development

### **Build Variants**
- **Debug** - Development build with logging
- **Release** - Optimized production build with ProGuard

### **Code Quality**
- **Kotlin Coding Conventions** - Following official guidelines
- **Clean Architecture** - Separation of concerns
- **SOLID Principles** - Maintainable and testable code
- **Documentation** - Comprehensive code documentation

### **Testing**
```bash
# Run unit tests
./gradlew test

# Run instrumented tests
./gradlew connectedAndroidTest
```

## 📱 Compatibility

- **Minimum SDK**: Android 7.0 (API level 24)
- **Target SDK**: Android 15 (API level 35)
- **Compile SDK**: Android 15 (API level 35)
- **Supported Languages**: English, Sanskrit
- **Screen Sizes**: Phone, Tablet, Foldable devices

## 🔒 Permissions

The app requires the following permissions:
- `INTERNET` - For fetching verse content and updates
- `ACCESS_NETWORK_STATE` - For checking network connectivity

## 🤝 Contributing

We welcome contributions to make this spiritual app even better!

### **How to Contribute**
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### **Contribution Guidelines**
- Follow Kotlin coding conventions
- Write meaningful commit messages
- Add appropriate documentation
- Test your changes thoroughly
- Respect the spiritual nature of the content

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **Bhagavad Gita Translations** - Various renowned scholars and translators
- **Sanskrit Resources** - Traditional texts and authentic sources
- **Open Source Libraries** - All the amazing libraries that make this app possible
- **Community** - Everyone who contributes to spreading spiritual knowledge

## 📞 Support

If you encounter any issues or have suggestions:

- **Email**: [your-email@domain.com]
- **GitHub Issues**: [Create an issue](https://github.com/yourusername/BhagavadGitaGyan/issues)
- **Discussions**: [Join our discussions](https://github.com/yourusername/BhagavadGitaGyan/discussions)

## 📈 Roadmap

### **Upcoming Features**
- [ ] Audio narration of verses
- [ ] Multiple language translations
- [ ] Advanced search functionality
- [ ] Daily notifications with verses
- [ ] Social sharing capabilities
- [ ] Offline mode improvements
- [ ] Meditation timer
- [ ] Progress tracking

---

<p align="center">
  <strong>🕉️ May this app bring peace, wisdom, and spiritual growth to all users 🕉️</strong>
</p>

<p align="center">
  Made with ❤️ and devotion for spreading the timeless wisdom of the Bhagavad Gita
</p>
