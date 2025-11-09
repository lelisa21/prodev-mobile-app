# 📱 ProDev Mobile App - React Native with Expo Router

A comprehensive React Native mobile application demonstrating advanced navigation patterns, component architecture, and modern styling with NativeWind (TailwindCSS). Built with Expo Router for seamless file-based routing and navigation.

[![React Native](https://img.shields.io/badge/React_Native-0.76+-61DAFB?style=for-the-badge&logo=react&logoColor=black)](https://reactnative.dev/)
[![Expo](https://img.shields.io/badge/Expo-52+-000020?style=for-the-badge&logo=expo&logoColor=white)](https://expo.dev/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.0+-3178C6?style=for-the-badge&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![Expo Router](https://img.shields.io/badge/Expo_Router-4.0+-000020?style=for-the-badge&logo=expo&logoColor=white)](https://docs.expo.dev/router/introduction/)
[![NativeWind](https://img.shields.io/badge/NativeWind-4.0+-38BDF8?style=for-the-badge&logo=tailwindcss&logoColor=white)](https://www.nativewind.dev/)

<div align="center">

### 🌟 Cross-Platform Mobile Excellence with React Native 🌟

*From Stack Navigation to NativeWind Styling - Building Modern Mobile Apps*

[Overview](#-project-overview) • [Quick Start](#-quick-start) • [Tasks](#-tasks-breakdown) • [Tech Stack](#-technologies-used) • [Resources](#-recommended-resources)

</div>

---

## 🎯 Project Overview

This project is part of the **ALX Professional Development** curriculum, focusing on advanced mobile app development with React Native and Expo Router. The project spans **four progressive tasks**, each building upon the previous to create a complete property listing mobile application.

### 🏆 Key Learning Objectives

- **File-Based Routing** with Expo Router v4
- **Stack & Tab Navigation** patterns
- **NativeWind Integration** (TailwindCSS for React Native)
- **Reusable Component Architecture** with TypeScript
- **Mobile-First UI/UX** implementation
- **Production-Ready** code structure

### 📱 What You'll Build

A property listing mobile application featuring:
- ✅ **Authentication Flow** - Landing, Sign In, Join screens
- ✅ **Tab Navigation** - Home, Search, Saved, Inbox, Profile
- ✅ **Property Listings** - Cards with ratings, favorites, and filtering
- ✅ **Modern Styling** - NativeWind utility-first CSS
- ✅ **TypeScript** - Type-safe development
- ✅ **Responsive Design** - Works on iOS & Android

---

## 📂 Repository Structure

```
prodev-mobile-app/
│
├── prodev-mobile-app-0x04/        # Task 0: Stack Navigation
│   ├── app/
│   │   ├── _layout.tsx            # Stack Navigator config
│   │   ├── index.tsx              # Landing page
│   │   ├── join.tsx               # Sign up screen
│   │   └── signin.tsx             # Login screen
│   ├── constants/
│   │   └── index.ts               # Image constants
│   ├── styles/
│   │   ├── _mainstyle.ts          # Main screen styles
│   │   └── _joinstyle.ts          # Auth screen styles
│   ├── assets/
│   │   └── images/                # App assets
│   ├── app.json
│   └── package.json
│
├── prodev-mobile-app-0x05/        # Task 1: Tab Navigation
│   ├── app/
│   │   ├── (home)/
│   │   │   ├── _layout.tsx        # Tab Navigator config
│   │   │   ├── index.tsx          # Home screen
│   │   │   ├── search.tsx         # Search screen
│   │   │   ├── saved.tsx          # Saved properties
│   │   │   ├── inbox.tsx          # Inbox screen
│   │   │   └── profile.tsx        # Profile screen
│   │   ├── index.tsx              # Landing page
│   │   ├── join.tsx               # Sign up
│   │   └── signin.tsx             # Login
│   ├── components/
│   │   ├── common/
│   │   │   └── PropertyListingCard.tsx
│   │   └── PropertyListing.tsx
│   ├── interfaces/
│   │   └── index.ts               # TypeScript interfaces
│   ├── constants/
│   │   ├── index.ts               # Image constants
│   │   └── data.ts                # Sample data
│   ├── styles/
│   │   ├── _mainstyle.ts
│   │   ├── _joinstyle.ts
│   │   ├── _homestyle.ts
│   │   └── _propertyCardStyle.ts
│   └── package.json
│
├── prodev-mobile-app-0x06/        # Task 2: NativeWind Styling
│   ├── app/
│   │   └── (home)/
│   │       └── profile.tsx        # Styled with Tailwind
│   ├── styles/
│   │   └── global.css             # Tailwind directives
│   ├── tailwind.config.js         # Tailwind config
│   ├── metro.config.js            # Metro bundler config
│   ├── babel.config.js            # Babel config
│   ├── nativewind-env.d.ts        # TypeScript defs
│   └── package.json
│
└── alx-[app-name]-app/            # Task 3: UI Challenge
    └── (Your chosen Figma implementation)
```

---

## 🚀 Quick Start

### Prerequisites

Before you begin, ensure you have:

- ✅ **Node.js** (v16 or higher) - [Download](https://nodejs.org/)
- ✅ **npm** or **yarn** package manager
- ✅ **Expo Go** app on your phone ([iOS](https://apps.apple.com/app/expo-go/id982107779) | [Android](https://play.google.com/store/apps/details?id=host.exp.exponent))
- ✅ **Git** for version control
- ✅ **Code Editor** (VS Code recommended)

### Installation Steps

```bash
# Clone the repository
git clone https://github.com/Dwaynemaster007/prodev-mobile-app.git
cd prodev-mobile-app

# Navigate to specific task directory
cd prodev-mobile-app-0x04

# Install dependencies
npm install

# Start development server
npx expo start

# Scan QR code with:
# • iOS: Camera app
# • Android: Expo Go app
```

### Project Setup from Scratch

```bash
# Create new Expo app (for reference)
npx create-expo-app@latest prodev-mobile-app-0x04

# Navigate to project
cd prodev-mobile-app-0x04

# Reset to clean slate
npm run reset-project

# Install dependencies
npm install

# Start development
npx expo start
```

---

## 📋 Tasks Breakdown

### Task 0: Stack Navigation Patterns 🔀

**Objective:** Implement Stack Navigation with authentication screens.

**Directory:** `prodev-mobile-app-0x04`

**What You'll Build:**
- Landing page with hero image and call-to-action buttons
- Join/Sign Up screen with form inputs
- Sign In screen with email/password fields
- Stack navigation between screens

**Key Concepts:**
- File-based routing with Expo Router
- Stack Navigator configuration
- StyleSheet objects for styling
- Image asset management
- TouchableOpacity for interactions

**Files Created:**
```
app/
├── _layout.tsx          # Stack configuration
├── index.tsx            # Landing page
├── join.tsx             # Sign up screen
└── signin.tsx           # Login screen

constants/index.ts       # Image constants
styles/
├── _mainstyle.ts        # Main screen styles
└── _joinstyle.ts        # Auth screen styles

assets/images/           # Hero images, logos
```

**Key Features:**
- ✅ Hero image background
- ✅ Company logo display
- ✅ Primary and secondary buttons
- ✅ Navigation between screens
- ✅ Consistent color scheme (#34967C primary)
- ✅ Reusable style constants

**Learning Outcomes:**
- Understand Expo Router file structure
- Implement Stack navigation
- Create reusable components
- Style with StyleSheet.create()
- Handle navigation actions

---

### Task 1: Tab Navigation with Property Listings 📱

**Objective:** Add Tab Navigation and build property listing components.

**Directory:** `prodev-mobile-app-0x05`

**What You'll Build:**
- Bottom tab navigation with 5 sections
- Home screen with property listings
- PropertyListingCard component
- Horizontal filter ScrollView
- Sample property data

**Key Concepts:**
- Tab Navigator with Expo Router
- Grouped routes with (home) folder
- Reusable components
- TypeScript interfaces
- Expo Vector Icons
- Component composition

**Files Created:**
```
app/(home)/
├── _layout.tsx          # Tab configuration
├── index.tsx            # Home with listings
├── search.tsx           # Search screen
├── saved.tsx            # Saved properties
├── inbox.tsx            # Messages
└── profile.tsx          # User profile

components/
├── PropertyListing.tsx
└── common/
    └── PropertyListingCard.tsx

interfaces/index.ts      # TypeScript types
constants/data.ts        # Sample data
styles/_propertyCardStyle.ts
```

**Tab Icons:**
- 🏠 Home - `AntDesign: home`
- 🔍 Search - `Feather: search`
- ❤️ Saved - `EvilIcons: heart`
- 💬 Inbox - `Ionicons: chatbubbles-outline`
- 👤 Profile - `FontAwesome: user-o`

**Property Card Features:**
- ✅ ImageBackground overlay
- ✅ Star rating display
- ✅ Property name and location
- ✅ Price tag with currency
- ✅ Favorite toggle button
- ✅ Gradient overlay effect

**Sample Data Structure:**
```typescript
interface PropertyListingProps {
  propertyName: string;
  rate: number;
  currency: string;
  amount: number;
  location: {
    street: string;
    city: string;
    country: string;
  };
  favorite: boolean;
  image?: string;
}
```

**Learning Outcomes:**
- Implement Tab navigation
- Build reusable card components
- Use TypeScript interfaces
- Integrate vector icons
- Create sample data
- Style complex layouts

---

### Task 2: NativeWind Styling (TailwindCSS) 🎨

**Objective:** Refactor Profile screen with NativeWind utility classes.

**Directory:** `prodev-mobile-app-0x06`

**What You'll Build:**
- Complete NativeWind setup
- Redesigned Profile screen with Tailwind classes
- Configuration files for proper integration
- Utility-first styling approach

**Key Concepts:**
- NativeWind installation and setup
- Tailwind utility classes in React Native
- Configuration files (tailwind, metro, babel)
- SafeAreaView with NativeWind
- Reduced code complexity

**Configuration Files:**

**`tailwind.config.js`**
```javascript
module.exports = {
  content: [
    "./App.{js,jsx,ts,tsx}",
    "./app/**/*.{js,jsx,ts,tsx}",
    "./components/**/*.{js,jsx,ts,tsx}"
  ],
  theme: {
    extend: {},
  },
  plugins: [],
}
```

**`metro.config.js`**
```javascript
const { getDefaultConfig } = require("expo/metro-config");
const { withNativeWind } = require('nativewind/metro');

const config = getDefaultConfig(__dirname);

module.exports = withNativeWind(config, { input: './styles/global.css' });
```

**`babel.config.js`**
```javascript
module.exports = function (api) {
  api.cache(true);
  return {
    presets: ['babel-preset-expo'],
    plugins: ["nativewind/babel"],
  };
};
```

**`styles/global.css`**
```css
@tailwind base;
@tailwind components;
@tailwind utilities;
```

**Profile Screen Features:**
- ✅ User info card with edit button
- ✅ Account settings section
- ✅ Security options (Face ID, 2FA)
- ✅ Additional settings section
- ✅ All styled with Tailwind classes
- ✅ SafeAreaView implementation

**Tailwind Classes Used:**
```typescript
// Container
className="flex-1 p-4"

// Flexbox
className="flex-row items-center gap-4"

// Colors & Backgrounds
className="bg-[#34967C] text-white"

// Typography
className="text-4xl font-semibold"

// Sizing & Spacing
className="w-12 h-12 p-4 mb-6"

// Borders & Radius
className="rounded-md border-2"
```

**Benefits of NativeWind:**
- ✅ **Less Code** - Fewer files and lines
- ✅ **Faster Development** - No StyleSheet objects
- ✅ **Consistency** - Design system built-in
- ✅ **Readability** - Styles with components
- ✅ **Flexibility** - Easy to modify

**Learning Outcomes:**
- Set up NativeWind in Expo
- Configure bundler and compiler
- Use Tailwind utility classes
- Refactor StyleSheet to className
- Understand utility-first CSS

---

### Task 3: UI Implementation Challenge 🎨

**Objective:** Build a complete app from Figma designs.

**Directory:** `alx-[app-name]-app`

**Choose One Design:**
1. **CoinPay App** - Cryptocurrency wallet
2. **Coffee Shop App** - Coffee ordering
3. **Online Groceries App** - Grocery shopping

**Requirements:**
- ✅ Initialize new Expo app with TypeScript
- ✅ Install NativeWind for styling
- ✅ Extract UI assets from Figma
- ✅ Implement all screens pixel-perfect
- ✅ Add smooth animations
- ✅ Document process in README
- ✅ Record demo video

**Deliverables:**
1. GitHub repository: `alx-[app-name]-app`
2. Complete implementation
3. README with process documentation
4. Demo video on social media
5. Tag & credit Figma designer

**Suggested Repository Names:**
```
alx-coinpay-app
alx-coffee-shop-app
alx-online-groceries-app
```

**Social Media Post Template:**
```
🚀 Just completed my React Native app challenge! 

Built [App Name] using:
• React Native & Expo Router
• TypeScript
• NativeWind (TailwindCSS)
• Pixel-perfect UI from Figma

Check out the demo! 📱✨

Design credit: [Designer Name]
#ReactNative #MobileDev #ALX #ExpoRouter

[Demo Video]
[GitHub Link]
```

**Evaluation Criteria:**
- ✅ Code quality and structure
- ✅ Pixel-perfect design implementation
- ✅ Smooth animations
- ✅ TypeScript usage
- ✅ Component reusability
- ✅ Documentation quality

**Learning Outcomes:**
- Translate Figma to code
- Build complete app from scratch
- Implement complex UI
- Add animations
- Document development process
- Share work professionally

---

## 🛠️ Technologies Used

### Core Technologies

**React Native Ecosystem:**
```json
{
  "react-native": "0.76.0",
  "react": "18.3.1",
  "expo": "~52.0.0",
  "expo-router": "~4.0.0"
}
```

**Styling:**
```json
{
  "nativewind": "^4.0.0",
  "tailwindcss": "^3.4.0"
}
```

**UI Components:**
```json
{
  "@expo/vector-icons": "^14.0.0",
  "react-native-safe-area-context": "4.12.0"
}
```

**Development:**
```json
{
  "typescript": "~5.3.3",
  "@types/react": "~18.3.12"
}
```

### Key Libraries

| Library | Purpose | Version |
|---------|---------|---------|
| **Expo** | Development platform | ~52.0.0 |
| **Expo Router** | File-based routing | ~4.0.0 |
| **NativeWind** | TailwindCSS for RN | ^4.0.0 |
| **TypeScript** | Type safety | ~5.3.3 |
| **Vector Icons** | Icon library | ^14.0.0 |
| **SafeArea Context** | Device compatibility | 4.12.0 |

---

## 📱 Core Components Reference

### Layout Components

```typescript
// View - Container component
<View style={styles.container}>
  {/* Content */}
</View>

// SafeAreaView - Avoid notches/bars
<SafeAreaView style={{ flex: 1 }}>
  {/* Safe content */}
</SafeAreaView>

// ScrollView - Scrollable container
<ScrollView>
  {/* Scrollable content */}
</ScrollView>
```

### Interactive Components

```typescript
// TouchableOpacity - Pressable with opacity feedback
<TouchableOpacity
  onPress={() => console.log('Pressed')}
  activeOpacity={0.7}
  style={styles.button}
>
  <Text>Press Me</Text>
</TouchableOpacity>

// Pressable - Advanced touch handling
<Pressable
  onPress={handlePress}
  style={({ pressed }) => [
    styles.button,
    pressed && styles.pressed
  ]}
>
  <Text>Advanced Press</Text>
</Pressable>
```

### Text & Input

```typescript
// Text - Display text
<Text style={styles.text}>Hello World</Text>

// TextInput - User input
<TextInput
  value={email}
  onChangeText={setEmail}
  placeholder="Enter email"
  keyboardType="email-address"
  autoCapitalize="none"
  secureTextEntry={isPassword}
  style={styles.input}
/>
```

### Media Components

```typescript
// Image - Display images
<Image
  source={require('./assets/logo.png')}
  style={styles.image}
  resizeMode="cover"
/>

// ImageBackground - Background image
<ImageBackground
  source={require('./assets/hero.png')}
  style={styles.background}
  resizeMode="cover"
>
  {/* Content over image */}
</ImageBackground>
```

---

## 🎨 Styling Approaches

### StyleSheet (Tasks 0-1)

```typescript
import { StyleSheet } from 'react-native';

const styles = StyleSheet.create({
  container: {
    flex: 1,
    backgroundColor: '#fff',
    padding: 20,
  },
  title: {
    fontSize: 24,
    fontWeight: '700',
    color: '#000',
    marginBottom: 16,
  },
  button: {
    backgroundColor: '#34967C',
    paddingVertical: 12,
    paddingHorizontal: 24,
    borderRadius: 8,
    alignItems: 'center',
  },
});
```

### NativeWind (Task 2+)

```typescript
// Same result with Tailwind classes
<View className="flex-1 bg-white p-5">
  <Text className="text-2xl font-bold text-black mb-4">
    Title
  </Text>
  <TouchableOpacity className="bg-[#34967C] py-3 px-6 rounded-lg items-center">
    <Text className="text-white">Button</Text>
  </TouchableOpacity>
</View>
```

**Comparison:**

| Aspect | StyleSheet | NativeWind |
|--------|-----------|------------|
| Setup | Built-in | Requires config |
| Code Volume | More files | Less code |
| Learning Curve | Easy | Tailwind knowledge |
| Consistency | Manual | Built-in system |
| Flexibility | High | Very High |
| Performance | Optimized | Optimized |

---

## 🔧 Available Commands

### Expo Commands

```bash
# Start development server
npx expo start

# Start with cleared cache
npx expo start --clear

# Platform specific
npx expo start --ios
npx expo start --android
npx expo start --web

# Tunnel for remote testing
npx expo start --tunnel

# Doctor (check environment)
npx expo-doctor

# Install Expo packages
npx expo install package-name
```

### Project Commands

```bash
# Install dependencies
npm install

# Reset project (clean slate)
npm run reset-project

# Run on platforms
npm run ios
npm run android
npm run web

# Lint code
npm run lint

# Type check
npx tsc --noEmit
```

### Git Commands

```bash
# Initialize repository
git init
git add .
git commit -m "feat(task-0): Initialize Stack navigation"

# Add remote
git remote add origin https://github.com/Dwaynemaster007/prodev-mobile-app.git

# Push to GitHub
git branch -M main
git push -u origin main
```

---

## 🐛 Common Issues & Solutions

### Metro Bundler Issues

```bash
# Clear cache and restart
npx expo start --clear

# Reset metro bundler
rm -rf node_modules/.cache
npx expo start -c

# Clear watchman (macOS)
watchman watch-del-all
```

### Expo Go Connection Problems

```bash
# Ensure same WiFi network
# Try tunnel connection
npx expo start --tunnel

# Or use LAN
npx expo start --lan

# Check firewall settings
```

### NativeWind Not Working

```bash
# Verify configuration files
# Check tailwind.config.js content paths
# Ensure babel.config.js has NativeWind plugin
# Restart metro bundler with cache clear
npx expo start --clear
```

### TypeScript Errors

```bash
# Regenerate tsconfig
npx expo customize tsconfig.json

# Install missing types
npm install --save-dev @types/react @types/react-native

# Restart TypeScript server in VS Code
# Cmd+Shift+P > TypeScript: Restart TS Server
```

### Image Not Showing

```typescript
// Check path is correct
source={require("@/assets/images/logo.png")}

// For remote images, add dimensions
<Image 
  source={{ uri: "https://example.com/img.png" }}
  style={{ width: 200, height: 200 }}
/>

// Check file exists in assets folder
// Check file extension matches (case-sensitive)
```

### Dependencies Installation Fails

```bash
# Clear npm cache
npm cache clean --force

# Remove and reinstall
rm -rf node_modules package-lock.json
npm install

# Try with legacy peer deps
npm install --legacy-peer-deps
```

---

## 💡 Best Practices

### Project Organization

```
app/
├── (auth)/              # Auth-related screens
│   ├── _layout.tsx
│   ├── signin.tsx
│   └── signup.tsx
├── (home)/              # Main app screens
│   ├── _layout.tsx
│   ├── index.tsx
│   └── profile.tsx
└── _layout.tsx          # Root layout

components/
├── common/              # Reusable components
│   ├── Button.tsx
│   ├── Card.tsx
│   └── Input.tsx
└── [feature]/           # Feature-specific

constants/
├── Colors.ts            # Color palette
├── Sizes.ts             # Sizing system
└── data.ts              # Sample data

interfaces/
└── index.ts             # TypeScript types

styles/
├── global.css           # Tailwind directives
└── [screen].ts          # Screen-specific styles
```

### Component Best Practices

```typescript
// 1. Use TypeScript interfaces
interface ButtonProps {
  title: string;
  onPress: () => void;
  variant?: 'primary' | 'secondary';
}

// 2. Extract reusable components
const Button: React.FC<ButtonProps> = ({ title, onPress, variant = 'primary' }) => {
  return (
    <TouchableOpacity onPress={onPress} style={styles[variant]}>
      <Text>{title}</Text>
    </TouchableOpacity>
  );
};

// 3. Use React.memo for performance
export default React.memo(Button);

// 4. Separate concerns
// ✅ Component logic in component
// ✅ Styles in StyleSheet or Tailwind
// ✅ Data in constants/data
// ✅ Types in interfaces
```

### Styling Best Practices

```typescript
// Define reusable constants
const COLORS = {
  primary: '#34967C',
  secondary: '#FFA800',
  text: '#0D0D0D',
  textLight: '#7E7B7B',
  background: '#FFFFFF',
};

const SPACING = {
  xs: 4,
  sm: 8,
  md: 16,
  lg: 24,
  xl: 32,
};

// Use consistent sizing
const FONT_SIZE = {
  small: 12,
  medium: 16,
  large: 20,
  xlarge: 24,
  xxlarge: 32,
};

// Apply in styles
const styles = StyleSheet.create({
  container: {
    padding: SPACING.lg,
    backgroundColor: COLORS.background,
  },
  title: {
    fontSize: FONT_SIZE.xlarge,
    color: COLORS.text,
  },
});
```

### Performance Optimization

```typescript
// Use FlatList for long lists
<FlatList
  data={items}
  renderItem={({ item }) => <ListItem item={item} />}
  keyExtractor={(item) => item.id}
  removeClippedSubviews={true}
  maxToRenderPerBatch={10}
  windowSize={10}
/>

// Use useCallback for functions
const handlePress = useCallback(() => {
  // Handle press
}, [dependencies]);

// Use useMemo for expensive calculations
const filteredData = useMemo(
  () => data.filter(item => item.active),
  [data]
);

// Optimize images
// - Use appropriate sizes
// - Compress before adding
// - Use caching for remote images
```

---

## 📚 Recommended Resources

### Official Documentation
- [React Native Docs](https://reactnative.dev/docs/getting-started) - Official React Native documentation
- [Expo Documentation](https://docs.expo.dev/) - Complete Expo platform guide
- [Expo Router](https://docs.expo.dev/router/introduction/) - File-based routing
- [NativeWind Docs](https://www.nativewind.dev/) - TailwindCSS for React Native

### Learning Platforms
- [React Native Express](https://www.reactnative.express/) - Interactive tutorials
- [freeCodeCamp React Native](https://www.youtube.com/watch?v=obH0Po_RdWk) - Complete course
- [Academind](https://academind.com/tutorials/react-native) - Video tutorials
- [React Native School](https://www.reactnativeschool.com/) - Premium courses

### Community Resources
- [React Native Directory](https://reactnative.directory/) - Library catalog
- [Expo Discord](https://chat.expo.dev/) - Community support
- [r/reactnative](https://www.reddit.com/r/reactnative/) - Reddit community
- [Stack Overflow](https://stackoverflow.com/questions/tagged/react-native) - Q&A

### YouTube Channels
- **Notjust.dev** - React Native tutorials and projects
- **The Net Ninja** - Complete beginner courses
- **Programming with Mosh** - Fundamentals and best practices
- **Simon Grimm** - Expo and React Native tips

### Design Resources
- [React Native Paper](https://reactnativepaper.com/) - Material Design
- [NativeBase](https://nativebase.io/) - Component library
- [Figma Community](https://www.figma.com/community) - Mobile UI kits
- [Dribbble](https://dribbble.com/tags/mobile-app) - Design inspiration

---

## 🎓 Learning Outcomes

By completing this project, you will master:

### Technical Skills
✅ **Expo Router** - File-based navigation system  
✅ **Stack Navigation** - Sequential screen flows  
✅ **Tab Navigation** - Bottom tab patterns  
✅ **NativeWind** - TailwindCSS in React Native  
✅ **TypeScript** - Type-safe development  
✅ **Component Architecture** - Reusable components  
✅ **State Management** - useState, props  
✅ **Asset Management** - Images and icons  
✅ **Responsive Design** - Cross-device layouts  
✅ **Vector Icons** - Icon integration

### Soft Skills
✅ **Problem Solving** - Debug and troubleshoot  
✅ **Code Organization** - Clean project structure  
✅ **Documentation** - Write clear README files  
✅ **Version Control** - Git workflow  
✅ **Testing** - Manual testing on devices  
✅ **UI/UX** - Mobile design principles  
✅ **Time Management** - Meet project deadlines  
✅ **Learning Ability** - Adapt to new tools

### Career Readiness
✅ **Portfolio Project** - Showcase to employers  
✅ **GitHub Presence** - Professional repositories  
✅ **Social Proof** - Demo videos and posts  
✅ **Technical Writing** - Documentation skills  
✅ **Best Practices** - Industry standards  
✅ **Full-Stack Mobile** - End-to-end development

---

## 🚀 Next Steps & Career Path

### Immediate Next Steps
1. **Navigation Advanced** - Deep linking, authentication flows
2. **State Management** - Redux, Zustand, Context API
3. **API Integration** - REST APIs, fetch, Axios
4. **Forms & Validation** - Formik, React Hook Form
5. **Async Storage** - Local data persistence

### Intermediate Level
6. **Authentication** - JWT, OAuth, social login
7. **Push Notifications** - Expo Notifications
8. **Maps & Location** - React Native Maps, geolocation
9. **Camera & Media** - Expo Camera, Image Picker
10. **Animations** - React Native Reanimated, Lottie

### Advanced Topics
11. **Native Modules** - Write custom native code
12. **Performance** - Profiling and optimization
13. **Testing** - Jest, Detox, React Native Testing Library
14. **CI/CD** - GitHub Actions, Fastlane
15. **Publishing** - App Store & Play Store deployment

### Career Opportunities

**Job Titles:**
- 📱 Mobile Developer
- 💼 React Native Developer
- 🚀 Cross-Platform Developer
- 🎨 Mobile UI/UX Developer
- 🔧 Full-Stack Mobile Engineer

**Companies Using React Native:**
- **Meta** (Facebook, Instagram)
- **Microsoft** (Outlook, Xbox)
- **Shopify** - E-commerce
- **Discord** - Communication
- **Bloomberg** - Finance
- **Coinbase** - Cryptocurrency
- **Uber Eats** - Food delivery
- **Airbnb** (parts of app)

**Salary Ranges** (2025 estimates):
- 🌱 **Junior** - $50,000 - $70,000/year
- 🌿 **Mid-Level** - $70,000 - $100,000/year
- 🌳 **Senior** - $100,000 - $150,000+/year
- 🚀 **Lead/Staff** - $150,000 - $200,000+/year

---

## 🤝 Contributing

While this is a learning project, feedback and suggestions are welcome!

### How to Contribute

1. **Fork the repository**
   ```bash
   # Click 'Fork' on GitHub
   ```

2. **Clone your fork**
   ```bash
   git clone https://github.com/yourusername/prodev-mobile-app.git
   cd prodev-mobile-app
   ```

3. **Create a feature branch**
   ```bash
   git checkout -b feature/your-improvement
   ```

4. **Make your changes**
   - Write clean, documented code
   - Follow existing code style
   - Test thoroughly on iOS and Android

5. **Commit your changes**
   ```bash
   git add .
   git commit -m "feat: Add your improvement description"
   ```

6. **Push to your fork**
   ```bash
   git push origin feature/your-improvement
   ```

7. **Open a Pull Request**
   - Describe your changes
   - Reference any related issues
   - Include screenshots if UI changes

### Contribution Guidelines

- ✅ Follow React Native best practices
- ✅ Use TypeScript for type safety
- ✅ Write descriptive commit messages
- ✅ Update documentation as needed
- ✅ Test on both iOS and Android
- ✅ Keep code clean and readable

---

## 📊 Project Timeline

**Duration:** November 2 - 16, 2025 (2 weeks)

```
Week 1: Nov 2-8, 2025
├── Day 1-2: Task 0 - Stack Navigation setup
├── Day 3-4: Task 1 - Tab Navigation implementation
└── Day 5-7: Task 2 - NativeWind integration

Week 2: Nov 9-16, 2025
├── Day 8-13: Task 3 - UI Challenge implementation
├── Day 14: Testing and refinement
├── Day 15: Documentation and demo video
└── Day 16: Submission and peer review
```

**Milestones:**
- ✅ **Week 1 Checkpoint** - Tasks 0-2 completed
- 🎯 **Week 2 Deliverable** - Task 3 with demo
- 📝 **Final Submission** - All tasks + documentation
- 👥 **Peer Review** - Request manual QA review

---

## 📈 Project Assessment

### Evaluation Criteria

**Code Quality (40%)**
- ✅ Clean, readable code
- ✅ Proper TypeScript usage
- ✅ Component reusability
- ✅ Error handling
- ✅ Best practices followed

**Functionality (30%)**
- ✅ All features working
- ✅ Navigation flows correctly
- ✅ Forms functional
- ✅ Responsive design
- ✅ Cross-platform compatibility

**UI/UX (20%)**
- ✅ Pixel-perfect implementation
- ✅ Smooth animations
- ✅ Intuitive navigation
- ✅ Consistent styling
- ✅ Professional appearance

**Documentation (10%)**
- ✅ Complete README
- ✅ Code comments
- ✅ Setup instructions
- ✅ Demo video
- ✅ Social media post

### Submission Requirements

**Required Files:**
```
✅ app/index.tsx, app/join.tsx, app/signin.tsx
✅ app/(home)/_layout.tsx, app/(home)/index.tsx
✅ app/(home)/profile.tsx (with NativeWind)
✅ components/PropertyListing.tsx
✅ components/common/PropertyListingCard.tsx
✅ styles/_mainstyle.ts, styles/_joinstyle.ts
✅ styles/_propertyCardStyle.ts, styles/global.css
✅ constants/index.ts, constants/data.ts
✅ interfaces/index.ts
✅ tailwind.config.js, metro.config.js, babel.config.js
✅ app.json, package.json
✅ assets/images/* (all required images)
✅ README.md (comprehensive documentation)
```

**Submission Process:**
1. ✅ Complete all tasks on time
2. 📄 Commit all required files
3. 🔗 Generate review link on platform
4. 👥 Request peer reviews
5. 📹 Share demo video on social media

**Important Notes:**
- ⚠️ **Deadline:** November 16, 2025 at 11:00 PM
- ⚠️ **Late submissions** cannot generate review links
- ⚠️ **Auto-check** verifies core files
- ⚠️ **Manual review** required for full score

---

## 🎬 Demo & Showcase

### Recording Your Demo

**What to Include:**
1. **App Launch** - Show splash screen
2. **Landing Page** - Hero image, buttons
3. **Authentication** - Sign in/Join flow
4. **Tab Navigation** - Switch between tabs
5. **Property Listings** - Scroll through cards
6. **Interactions** - Tap favorites, filters
7. **Profile Screen** - Show NativeWind styling
8. **Both Platforms** - iOS and Android if possible

**Recording Tools:**
- **iOS:** Built-in Screen Recording
- **Android:** Built-in Screen Recorder
- **Editing:** iMovie, CapCut, DaVinci Resolve

### Social Media Template

**LinkedIn Post:**
```
🎉 Excited to share my latest React Native project!

I just completed a property listing mobile app as part of the ALX ProDev curriculum. Built from scratch using:

📱 React Native & Expo Router
⚡ TypeScript for type safety
🎨 NativeWind (TailwindCSS)
🧭 Stack & Tab Navigation
🏗️ Reusable component architecture

Key features:
✅ Cross-platform (iOS & Android)
✅ Property cards with ratings & favorites
✅ Smooth navigation flows
✅ Modern, clean UI
✅ Responsive design

This project taught me advanced mobile development patterns and reinforced the importance of clean code architecture.

Check out the demo video and feel free to connect if you're interested in mobile development!

#ReactNative #MobileDevelopment #ALX #ExpoRouter #NativeWind #TypeScript #CrossPlatform

[Link to GitHub]
[Demo Video]
```

**Twitter/X Post:**
```
🚀 Just shipped a React Native app!

Built a property listing app with:
📱 Expo Router
⚡ TypeScript
🎨 NativeWind
🧭 Stack & Tab Nav

One codebase → iOS + Android ✨

#ReactNative #100DaysOfCode

[Demo Video]
[GitHub Link]
```

**Instagram/TikTok Caption:**
```
📱 Building mobile apps with React Native! 

Swipe to see the process ➡️

Stack: React Native, Expo, TypeScript, TailwindCSS

#MobileDev #ReactNative #CodingLife #TechTok
```

---

## 🔒 Security Best Practices

### Environment Variables

```bash
# Never commit sensitive data
# Create .env file (add to .gitignore)
API_KEY=your_api_key_here
API_URL=https://api.example.com

# Access in code
import Constants from 'expo-constants';

const apiKey = Constants.expoConfig?.extra?.apiKey;
```

### Secure Storage

```bash
# Install secure storage
npx expo install expo-secure-store

# Use for tokens, passwords
import * as SecureStore from 'expo-secure-store';

await SecureStore.setItemAsync('userToken', token);
const token = await SecureStore.getItemAsync('userToken');
```

### Best Practices Checklist

- ✅ Never hardcode API keys
- ✅ Use HTTPS for all network requests
- ✅ Validate user input
- ✅ Implement proper authentication
- ✅ Use secure storage for sensitive data
- ✅ Keep dependencies updated
- ✅ Follow principle of least privilege
- ✅ Log errors, not sensitive data

---

## 📱 Testing Checklist

### Manual Testing

**Stack Navigation (Task 0)**
- [ ] Landing page displays correctly
- [ ] Hero image loads properly
- [ ] Buttons navigate to correct screens
- [ ] Join screen form is accessible
- [ ] Sign in screen form is accessible
- [ ] Back navigation works
- [ ] Layout looks good on different devices

**Tab Navigation (Task 1)**
- [ ] All 5 tabs are visible
- [ ] Tab icons display correctly
- [ ] Active tab is highlighted
- [ ] Home screen shows property listings
- [ ] Property cards display all information
- [ ] Favorite icon toggles (visual)
- [ ] Scroll works smoothly
- [ ] Filter chips are scrollable horizontally
- [ ] Show more button is visible

**NativeWind Styling (Task 2)**
- [ ] Profile screen uses Tailwind classes
- [ ] User card displays correctly
- [ ] Icons are properly sized and colored
- [ ] Settings sections are organized
- [ ] Pressable items respond to touch
- [ ] Layout is responsive
- [ ] SafeArea is implemented
- [ ] Colors match design (#34967C, etc.)

**Cross-Platform**
- [ ] Test on iOS device/simulator
- [ ] Test on Android device/emulator
- [ ] Check different screen sizes
- [ ] Verify safe areas work correctly
- [ ] Test portrait orientation
- [ ] Check status bar appearance
- [ ] Verify touch targets are adequate

**Performance**
- [ ] App starts quickly
- [ ] No lag when scrolling
- [ ] Images load efficiently
- [ ] Transitions are smooth
- [ ] No memory leaks
- [ ] Hot reload works properly

---

## 📖 Additional Resources

### Figma Designs (Task 3)

**CoinPay App**
- Modern cryptocurrency wallet UI
- Features: Wallet, transactions, charts
- Design credit: [Figma Community]

**Coffee Shop App**
- Coffee ordering and menu UI
- Features: Menu, cart, orders
- Design credit: [Figma Community]

**Online Groceries App**
- Grocery shopping experience
- Features: Products, cart, checkout
- Design credit: [Figma Community]

### Asset Resources

**Icons:**
- [Expo Vector Icons](https://icons.expo.fyi/) - Browse all icons
- [Flaticon](https://www.flaticon.com/) - Free icons
- [Icons8](https://icons8.com/) - Icon library

**Images:**
- [Unsplash](https://unsplash.com/) - Free stock photos
- [Pexels](https://www.pexels.com/) - Free images and videos
- [Pixabay](https://pixabay.com/) - Free media

**Fonts:**
- [Google Fonts](https://fonts.google.com/) - Free fonts
- [Expo Google Fonts](https://github.com/expo/google-fonts) - Integration

### Useful Tools

**Development:**
- [React Native Debugger](https://github.com/jhen0409/react-native-debugger)
- [Reactotron](https://github.com/infinitered/reactotron)
- [Expo DevTools](https://docs.expo.dev/workflow/debugging/)

**Design:**
- [Figma](https://www.figma.com/) - UI design tool
- [Sketch](https://www.sketch.com/) - Design platform
- [Adobe XD](https://www.adobe.com/products/xd.html) - UX design

**Code Quality:**
- [ESLint](https://eslint.org/) - Linting
- [Prettier](https://prettier.io/) - Code formatting
- [TypeScript](https://www.typescriptlang.org/) - Type checking

---

## 📞 Support & Contact

### Get Help

**Project Issues:**
- 🐛 [Open an Issue](https://github.com/Dwaynemaster007/prodev-mobile-app/issues)
- 💬 ALX Slack Channel
- 📧 Peer support

**Technical Questions:**
- [Stack Overflow](https://stackoverflow.com/questions/tagged/react-native)
- [Expo Forums](https://forums.expo.dev/)
- [React Native Discord](https://www.reactiflux.com/)

### Author Contact

**Thubelihle Dlamini (Dwaynemaster007)**

- 📧 **Email:** [thubelihledlamini88@gmail.com](mailto:thubelihledlamini88@gmail.com)
- 💼 **LinkedIn:** [linkedin.com/in/thubelihledlamini](https://www.linkedin.com/in/thubelihledlamini/)
- 🐦 **Twitter/X:** [@dwaynemaster](https://twitter.com/dwaynemaster)
- 💻 **GitHub:** [@Dwaynemaster007](https://github.com/Dwaynemaster007)

**Response Time:**
- Usually within 24-48 hours
- Faster on ALX Slack
- Check GitHub issues first

---

## 📄 License

This project is part of the **ALX Professional Development Frontend Curriculum**.

**Usage Rights:**
- ✅ Use for learning and portfolio
- ✅ Modify and experiment
- ✅ Share with attribution
- ❌ Commercial use without permission
- ❌ Claim as original work

© 2025 ALX Africa. Educational use permitted.

---

## 🙏 Acknowledgments

### Special Thanks To

**ALX Africa**
- For providing comprehensive curriculum
- For supporting learning journey
- For creating opportunities

**Community Contributors**
- Expo team for excellent documentation
- React Native community for resources
- Open source contributors

**Design Credits**
- Figma designers for UI inspirations
- Icon designers for visual assets
- Stock photo providers

**Mentors & Peers**
- ALX instructors for guidance
- Peer reviewers for feedback
- Study group members for support

---

## 🏆 Project Showcase

### What Makes This Project Stand Out

**Technical Excellence:**
- ✅ Modern stack (Expo Router, NativeWind)
- ✅ TypeScript for reliability
- ✅ Clean architecture
- ✅ Best practices throughout
- ✅ Cross-platform compatibility

**User Experience:**
- ✅ Intuitive navigation
- ✅ Smooth interactions
- ✅ Professional design
- ✅ Responsive layouts
- ✅ Attention to detail

**Code Quality:**
- ✅ Well-organized structure
- ✅ Reusable components
- ✅ Comprehensive documentation
- ✅ Type-safe implementation
- ✅ Scalable architecture

**Learning Demonstration:**
- ✅ Progressive complexity
- ✅ Multiple patterns
- ✅ Problem-solving skills
- ✅ Adaptability
- ✅ Professional workflow

---

## 🎯 Key Takeaways

### What You've Mastered

**Mobile Development Fundamentals:**
1. ✅ Expo ecosystem and workflow
2. ✅ React Native core components
3. ✅ File-based routing with Expo Router
4. ✅ Stack and Tab navigation patterns
5. ✅ Cross-platform development

**Component Architecture:**
6. ✅ Reusable component design
7. ✅ Props and TypeScript interfaces
8. ✅ Component composition
9. ✅ Separation of concerns
10. ✅ Clean code principles

**Styling Approaches:**
11. ✅ StyleSheet methodology
12. ✅ NativeWind/TailwindCSS
13. ✅ Responsive design
14. ✅ Design systems
15. ✅ Utility-first CSS

**Professional Skills:**
16. ✅ Git version control
17. ✅ Project documentation
18. ✅ Code organization
19. ✅ Testing and debugging
20. ✅ Portfolio presentation

---

## 🌟 Success Metrics

### Project Completion Indicators

**Technical Completion:**
- ✅ All 4 tasks implemented
- ✅ All screens functional
- ✅ Navigation working correctly
- ✅ Styling applied properly
- ✅ TypeScript without errors
- ✅ Runs on iOS and Android

**Quality Metrics:**
- ✅ Code is clean and readable
- ✅ Components are reusable
- ✅ No console errors
- ✅ Smooth performance
- ✅ Professional appearance
- ✅ Responsive design

**Documentation:**
- ✅ README is comprehensive
- ✅ Code has comments
- ✅ Setup instructions clear
- ✅ Demo video recorded
- ✅ Social media shared

**Learning Outcomes:**
- ✅ Understanding of Expo Router
- ✅ Mastery of navigation patterns
- ✅ Confidence with NativeWind
- ✅ TypeScript proficiency
- ✅ Mobile development skills

---

## 🚀 Ready to Get Started?

### Quick Start Commands

```bash
# Clone and start Task 0
git clone https://github.com/Dwaynemaster007/prodev-mobile-app.git
cd prodev-mobile-app/prodev-mobile-app-0x04
npm install
npx expo start

# Or create from scratch
npx create-expo-app@latest my-app
cd my-app
npm run reset-project
npx expo start
```

### Your Learning Path

```
1. Complete Task 0 → Stack Navigation ✅
2. Complete Task 1 → Tab Navigation ✅
3. Complete Task 2 → NativeWind Styling ✅
4. Complete Task 3 → UI Challenge 🎨
5. Record Demo Video 📹
6. Update Documentation 📝
7. Submit & Share 🚀
```

---

<div align="center">

## 💜 Built with React Native Excellence 💜

### *From Landing to Deployment - One Component at a Time* 📱✨

**Made with 💚 by [Thubelihle Dlamini (Dwaynemaster007)](https://github.com/Dwaynemaster007)**

---

[![GitHub](https://img.shields.io/badge/GitHub-Dwaynemaster007-181717?style=for-the-badge&logo=github)](https://github.com/Dwaynemaster007)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Thubelihle_Dlamini-0077B5?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/thubelihledlamini/)
[![Twitter](https://img.shields.io/badge/Twitter-@dwaynemaster-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://twitter.com/dwaynemaster)
[![Email](https://img.shields.io/badge/Email-thubelihledlamini88-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:thubelihledlamini88@gmail.com)

---

### 🏷️ Repository Tags

`react-native` • `expo` • `expo-router` • `typescript` • `nativewind` • `tailwindcss` • `mobile-development` • `cross-platform` • `ios` • `android` • `stack-navigation` • `tab-navigation` • `property-listing` • `ui-components` • `alx-africa` • `prodev` • `mobile-app` • `frontend` • `javascript` • `react` • `learning-project` • `portfolio` • `beginner-friendly` • `tutorial`

---

**Project Status:** ✅ Complete | 🎯 Ready for Review | 🚀 Production Ready

**Last Updated:** November 2025

**License:** Educational Use - ALX Africa

---

### ⭐ If this project helped you, please give it a star! ⭐

</div>