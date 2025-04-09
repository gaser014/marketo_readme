# Marketo: The Ultimate E-Commerce Admin and User Flutter App

Marketo provides an all-in-one Flutter application tailored for both admin and user roles .It is designed to simplify
e-commerce management and enhance user experiences .With its comprehensive features, this app enables admins to
efficiently manage their platform while providing users with a seamless shopping experience.

## Administrative Interface

### Features Overview

- **Product Management**:
    - Add, edit, and remove products
    - Manage product variants and pricing
    - Upload product images and descriptions
    - Track inventory levels

- **Category Management**:
    - Create and organize main categories
    - Manage sub-categories
    - Link products to appropriate categories

- **Promotional Tools**:
    - Create and manage special offers
    - Generate and track coupon codes
    - Design promotional sliders
    - Configure homepage featured sections

- **Order Management**:
    - Track all incoming orders
    - Update order status
    - Monitor delivery progress
    - Access order history and analytics

### Key Administrative Screens

1. Dashboard Overview
2. Product Management Console
3. Category Configuration
4. Offer Management
5. Coupon Administration
6. Order Tracking System
7. Slider Configuration
8. Analytics and Reports

## Customer Interface

### Features Overview

- **Personalized Shopping Experience**:
    - Browse dynamic homepage sliders
    - Explore categorized products
    - View special offers and deals
    - Access personalized recommendations

- **Product Discovery**:
    - Browse by categories and subcategories
    - Search products by name
    - Filter products by various attributes
    - View "Best Seller" collections
    - Explore "New Arrivals"

- **Shopping Features**:
    - Detailed product pages with variants
    - Shopping cart management
    - Coupon application system
    - Order tracking capabilities

### Key Customer Screens

1. Home Screen (with sliders and featured sections)
2. Category Browse
3. Product Search
4. Product Details
5. Shopping Cart
6. Checkout Process
7. Order History
8. Account Management

## Technical Specifications

### Multilingual Support

- Arabic (ar)
- English (en)
- French (fr)
- German (de)

### Order Processing

1. Product selection with variant options
2. Shopping cart management
3. Coupon application
4. Shipping information collection
5. Order confirmation with unique ID
6. Status tracking

### Integration Requirements

- Backend documentation review required for admin account setup
- API integration for product and order management
- Database configuration for multi-language support
- A secure authentication system for both interfaces

## How to Get and Run the App

Follow these steps to set up and run the e-commerce app on your local machine:

### Prerequisites

1. Ensure you have Flutter installed on your system. Follow the installation guide
   at [Flutter.dev](https://flutter.dev/docs/get-started/install).
2. Install an editor like [VS Code](https://code.visualstudio.com/)
   or [Android Studio](https://developer.android.com/studio).
3. Set up an Android emulator or connect a physical device.

### Steps to Get and Run the App on Your Local Machine

1. Clone the repository
2. Navigate to the project directory
3. Fetch the dependencies by running "flutter pub get"
4. Run the app on your connected device or emulator by running "flutter run
### Steps to add new language
      you can add a new language by following these steps or you can check the todo list in the project to see the steps in lib/core/enum/enums.dart, main.dart and my_app.dart
1. Add a new JSON file in the assets/lang folder with the language code as the filename (e.g., fr.json for French).
2. Add the translations in the JSON file in the following format:
```json
{
  "key": "value",
  "key2": "value2"
}
```
you can use en.json as a reference.
3. Update the supportedLocales list in the main.dart and my_app file with the new language code.
4. Add the new language to the dropdown by updating the languageList in lib/core/enum/enums.dart
