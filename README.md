# SOCIAL SAVER DONWLOADER (SOCIAL SAVER SDK)

A simple Node.js tool to generate direct download links for media from **Instagram**, **Facebook**, **Twitter (X)**, **Snapchat**, **TikTok**, and **Pinterest**!  
Just provide the post URL, and this package will return the direct media download URL.

---

## 🔐 Authentication Required

This SDK is **paid and protected**.  
To use any downloader function, you must pass a valid `authToken`.

### How to Get an `authToken`:
- 🌐 Visit: [https://happykumar.com](https://happykumar.com)
- 📧 Email: **happykumar.info@gmail.com**

> All requests without a valid token will be denied.

---

## 🚀 Installation

Install via **npm**:

```bash
npm install github:ImHappyKumar/social-saver-sdk
```

Or, if you're using Yarn:

```bash
yarn add github:ImHappyKumar/social-saver-sdk
```

## Usage

### Importing the Package

You can import the entire `social-saver-sdk` module:

```javascript
const socialSaver = require("social-saver-sdk");
```

Or destructure specific functions:

```javascript
const {
  instagramDownloader,
  facebookDownloader,
  twitterDownloader,
  snapchatDownloader,
  tiktokDownloader,
  pinterestDownloader,
} = require("social-saver-sdk");
```

### Example Usage

#### Instagram Downloader

```javascript
async function fetchInstagramData() {
  try {
    const result = await socialSaver.instagramDownloader(
      "https://www.instagram.com/example-url"
    );
    console.log("Fetched Instagram media details:", result);
  } catch (error) {
    console.error("Error fetching Instagram media details:", error);
  }
}

fetchInstagramData();
```

#### Facebook Downloader

```javascript
async function fetchFacebookData() {
  try {
    const result = await socialSaver.facebookDownloader(
      "https://www.facebook.com/example-url"
    );
    console.log("Fetched Facebook media details:", result);
  } catch (error) {
    console.error("Error fetching Facebook media details:", error);
  }
}

fetchFacebookData();
```

#### Twitter Downloader

```javascript
async function fetchTwitterData() {
  try {
    const result = await socialSaver.twitterDownloader(
      "https://x.com/example-url"
    );
    console.log("Fetched Twitter media details:", result);
  } catch (error) {
    console.error("Error fetching Twitter media details:", error);
  }
}

fetchTwitterData();
```

#### Snapchat Downloader

```javascript
async function fetchSnapchatData() {
  try {
    const result = await socialSaver.snapchatDownloader(
      "https://snapchat.com/example-url"
    );
    console.log("Fetched Snapchat media details:", result);
  } catch (error) {
    console.error("Error fetching Snapchat media details:", error);
  }
}

fetchSnapchatData();
```

#### TikTok Downloader

```javascript
async function fetchTiktokData() {
  try {
    const result = await socialSaver.tiktokDownloader(
      "https://www.tiktok.com/example-url"
    );
    console.log("Fetched TikTok media details:", result);
  } catch (error) {
    console.error("Error fetching TikTok media details:", error);
  }
}

fetchTiktokData();
```

#### Pinterest Downloader

```javascript
async function fetchPinterestData() {
  try {
    const result = await socialSaver.pinterestDownloader(
      "https://in.pinterest.com/example-url"
    );
    console.log("Fetched Pinterest media details:", result);
  } catch (error) {
    console.error("Error fetching Pinterest media details:", error);
  }
}

fetchPinterestData();
```

## Supported Platforms

- Instagram
- Facebook
- Twitter
- Snapchat
- TikTok
- Pinterest

## 🧪 Express Router Integration

If you're using Express and want to quickly test the endpoints using the built-in router:

```javascript
const express = require("express");
const { router } = require("social-saver-sdk");

const app = express();
const PORT = 3000;

// Use the router at /test
app.use("/test", router);

app.listen(PORT, () => {
  console.log(`Server running on http://localhost:${PORT}`);
});
```

## Contributing

Contributions are welcome! If you find any issues or want to contribute new features, feel free to fork the repository and create a pull request.

### Steps to Contribute:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes and commit them (`git commit -am 'Add new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Create a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
