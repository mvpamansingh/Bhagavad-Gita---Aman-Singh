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

## 📱 Screenshots

<table>
  <tr>
    <td><img src="https://github.com/user-attachments/assets/16955624-1bbe-40b3-9c60-bd0379c2b53d" alt="Screenshot 1" width="250"/></td>
    <td><img src="https://github.com/user-attachments/assets/7fa66eda-1b01-4c6e-8ef3-e29bc49d2283" alt="Screenshot 2" width="250"/></td>
    <td><img src="https://github.com/user-attachments/assets/2bbc7477-2dfc-4e9f-be8c-788a64b1af92" alt="Screenshot 3" width="250"/></td>
  </tr>
  <tr>
    <td><img src="https://github.com/user-attachments/assets/e028c45c-c1e4-412d-8e81-c9caed1f3f44" alt="Screenshot 4" width="250"/></td>
    <td><img src="https://github.com/user-attachments/assets/f4c92a33-80c6-4435-865a-336cd1c4e66a" alt="Screenshot 5" width="250"/></td>
    <td><img src="https://github.com/user-attachments/assets/87e662b9-74ab-428f-ad16-22621e017eaf" alt="Screenshot 6" width="250"/></td>
  </tr>
</table>

## ✨ Features

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
- **Save Chapters**: Bookmark entire chapters for easy access which includes all verses
- **Verse Bookmarks**: Mark individual verses for reference
- **Personal Library**: Organize your saved spiritual content
- **Quick Access**: Navigate directly to bookmarked content

### 🏛️ **Virtual Temple**
- **Sacred Experience**: Create a divine atmosphere for meditation
- **Interactive Elements**: Perform Aarti song animation, offer flowers, ring bells, play bhajans
- **Peaceful Interface**: Designed for contemplation and prayer

### 📚 **Krishna Leela Stories**
- **Divine Pastimes**: Explore stories from Krishna's life
- **Chapter Organization**: Well-structured narrative content
- **Rich Storytelling**: Engaging presentation of sacred tales



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

### **Backend**
- **Nodejs**- Utilized as the runtime environment for server-side development
- **express**- Employed as the web application framework to build and manage the server
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

**Visit Playstore** - https://play.google.com/store/apps/details?id=com.mvpamansingh.shrimadbhagavadgita



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

## 🔧 Development

### **Build Variants**
- **Debug** - Development build with logging
- **Release** - Optimized production build with ProGuard

### **Code Quality**
- **Kotlin Coding Conventions** - Following official guidelines
- **Clean Architecture** - Separation of concerns
- **SOLID Principles** - Maintainable and testable code
- **Documentation** - Comprehensive code documentation



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


## 📞 Support

If you encounter any issues or have suggestions:

- **Email**: [amansingh.as9@outlook.com]


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
