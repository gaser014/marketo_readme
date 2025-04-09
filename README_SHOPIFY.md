# Marketo Shopify: The Ultimate E-Commerce User Flutter App

Marketo delivers a seamless Flutter application tailored for users, enhancing their shopping experience. Designed to integrate with Shopify, it provides a clean and efficient platform for browsing and purchasing products.

## Customer Interface

### Features Overview

- **Personalized Shopping Experience**:
    - Explore categorized products
    - Access personalized recommendations based on browsing history

- **Product Discovery**:
    - Browse by main categories
    - Search products by name
    - Filter products by various attributes
    - View "Limited Quantity"
    - Explore "New Arrivals"

- **Shopping Features**:
    - Detailed product pages with variants
    - Shopping cart management
    - Coupon application system
    - Order tracking capabilities

### Key Customer Screens

1. Home Screen
2. Category Browse
3. Product Search
4. Product Details
5. Shopping Cart
6. Checkout Process With Shopify 
7. Order History
8. Account Management

## Technical Specifications

### Multilingual Support

- Arabic (ar)
- English (en)

### Order Processing

1. Product selection with variant options
2. Shopping cart management
3. Coupon application
4. Shipping information collection
5. Order confirmation with unique ID
6. Status tracking


## **Integration with Shopify**

To integrate with Shopify, follow these steps:

- **Develop App in Shopify**:
    - Navigate to **Settings** -> **Apps** -> **App Development** -> **Create an App**.
    - Add any name for the app and click **Create App**.
- **Generate Access Tokens**:
    - For the newly created app, generate:
        - **X-Shopify-Access-Token**
        - **X-Shopify-Storefront-Access-Token**

    - **Configure API Permissions**:
        - Go to your app's configuration and ensure you have permissions for example:
            - **read_products**
            - **write_products**
            - **read_collections**
            - **write_collections**

These tokens and permissions will be used to interact with Shopify's API to fetch products, manage orders, and handle user data, allowing you to add your products and collections to the app channel.

### **Key Differences:**

| **Token Type**               | **Admin API Token**                     | **Storefront API Token**                |
|------------------------------|------------------------------------------|------------------------------------------|
| **Usage**                    | Backend operations (REST/GraphQL)        | Frontend customer interactions (GraphQL)|
| **Example Header**           | `X-Shopify-Access-Token`                 | `X-Shopify-Storefront-Access-Token`     |
| **Access**                   | Full store management                    | Limited to storefront data              |

---

Now, to add the TODO in the `lib/core/databases/graphql/graph_ql.dart` file, including the new permissions and the addition of products and collections:

## How to Get and Run the App

### Prerequisites

1. Ensure you have Flutter installed on your system. Follow the installation guide at [Flutter.dev](https://flutter.dev/docs/get-started/install).
2. Install an editor like [VS Code](https://code.visualstudio.com/) or [Android Studio](https://developer.android.com/studio).
3. Set up an Android emulator or connect a physical device.

### Steps to Get and Run the App on Your Local Machine

1. Clone the repository.
2. Navigate to the project directory.
3. Fetch the dependencies by running `flutter pub get`.
4. Run the app on your connected device or emulator by executing `flutter run`.

### Steps to Add a New Language

You can add a new language by following these steps or check the TODO list in the project:

1. Add a new JSON file in the `assets/lang` folder with the language code as the filename (e.g., `fr.json` for French).
2. Add translations in the JSON file in the following format:
   ```json
   {
     "key": "value",
     "key2": "value2"
   }
   ```
   Use `en.json` as a reference.
3. Update the `supportedLocales` list in `main.dart` and `my_app.dart` with the new language code.
4. Add the new language to the dropdown by updating the `languageList` in `lib/core/enum/enums.dart`.
