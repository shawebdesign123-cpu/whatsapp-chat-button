# Floating WhatsApp Chat Button

A simple, responsive floating WhatsApp chat button built with **HTML, CSS, and SVG**. Add a WhatsApp contact button to your website so visitors can start a conversation with your business using a pre-filled message.

## 🚀 Live Demo

**Click below to preview the live project.**

[![Live Demo](https://img.shields.io/badge/Live-Demo-25D366?style=for-the-badge&logo=googlechrome&logoColor=white)](https://shawebdesign.com/)

🔗 **Preview:** [https://shawebdesign.com/](https://shawebdesign.com/)

## ✨ Features

- Floating WhatsApp button fixed to the bottom-right corner.
- Opens a direct WhatsApp chat using the Click to Chat URL.
- Supports customizable pre-filled messages.
- Responsive design for desktop and mobile devices.
- Custom SVG WhatsApp icon without additional icon libraries.
- Smooth hover animation and shadow effects.
- Easy integration with HTML, PHP, and WordPress websites.
- Accessible label and keyboard focus styling.

## 🛠️ Technologies Used

- HTML5
- CSS3
- SVG
- WhatsApp Click to Chat

## 📦 Installation and Setup

### Step 1: Create Your WhatsApp Link

WhatsApp Click to Chat allows visitors to open a conversation with your business without saving your phone number.

**Format your phone number**

Use your country code followed by your phone number, without the `+` sign, spaces, hyphens, or leading zeros.

Example for Sri Lanka:

- Local number: `071 234 5678`
- International format: `94712345678`

**Basic WhatsApp link**

```text
https://wa.me/94712345678
```

**WhatsApp link with a pre-filled message**

```text
https://wa.me/94712345678?text=Hello%20Priyadi%20Nature%20Food%2C%20I%20have%20an%20inquiry%20about%20your%20products
```

Replace the example phone number and message with your business details.

### Step 2: Add the HTML

Add the following HTML to your website template, preferably before the closing `</body>` tag.

```html
<!-- Floating WhatsApp Button -->
<a
  href="https://wa.me/94712345678?text=Hello%20Priyadi%20Nature%20Food%2C%20I%20have%20an%20inquiry%20about%20your%20products"
  class="whatsapp-float"
  target="_blank"
  rel="noopener noreferrer"
  aria-label="Chat with us on WhatsApp"
>
  <svg
    xmlns="http://www.w3.org/2000/svg"
    width="32"
    height="32"
    viewBox="0 0 24 24"
    fill="#ffffff"
    aria-hidden="true"
  >
    <path d="M.057 24l1.687-6.163c-1.041-1.804-1.588-3.849-1.587-5.946.003-6.556 5.338-11.891 11.893-11.891 3.181.001 6.167 1.24 8.413 3.488 2.245 2.248 3.481 5.236 3.48 8.414-.003 6.557-5.338 11.892-11.893 11.892-1.99-.001-3.951-.5-5.688-1.448l-6.305 1.654zm6.597-3.807c1.676.995 3.276 1.591 5.392 1.592 5.448 0 9.886-4.434 9.889-9.885.002-5.462-4.415-9.89-9.881-9.892-5.452 0-9.887 4.434-9.889 9.884-.001 2.225.651 3.891 1.746 5.634l-.999 3.648 3.742-.981zm11.387-5.464c-.074-.124-.272-.198-.57-.347-.297-.149-1.758-.868-2.031-.967-.272-.099-.47-.149-.669.149-.198.297-.768.967-.941 1.165-.173.198-.347.223-.644.074-.297-.149-1.255-.462-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.297-.347.446-.521.151-.172.2-.296.3-.495.099-.198.05-.372-.025-.521-.075-.148-.669-1.611-.916-2.206-.242-.579-.487-.501-.669-.51l-.57-.01c-.198 0-.52.074-.792.372s-1.04 1.016-1.04 2.479 1.065 2.876 1.213 3.074c.149.198 2.095 3.2 5.076 4.487.709.306 1.263.489 1.694.626.712.226 1.36.194 1.872.118.571-.085 1.758-.719 2.006-1.413.248-.695.248-1.29.173-1.414z"/>
  </svg>
</a>
```

### Step 3: Add the CSS

Add the following styles to your main stylesheet, such as `style.css`.

```css
/* Floating WhatsApp Button */
.whatsapp-float {
  position: fixed;
  width: 60px;
  height: 60px;
  bottom: 25px;
  right: 25px;
  background-color: #25d366;
  color: #ffffff;
  border-radius: 50%;
  text-align: center;
  box-shadow: 2px 2px 8px rgba(0, 0, 0, 0.25);
  z-index: 9999;
  display: flex;
  align-items: center;
  justify-content: center;
  text-decoration: none;
  transition:
    background-color 0.3s ease,
    transform 0.3s ease,
    box-shadow 0.3s ease;
}

/* Hover Effect */
.whatsapp-float:hover {
  background-color: #128c7e;
  transform: scale(1.1);
  box-shadow: 2px 2px 12px rgba(0, 0, 0, 0.35);
}

/* Keyboard Accessibility */
.whatsapp-float:focus-visible {
  outline: 3px solid #128c7e;
  outline-offset: 4px;
}

/* Mobile Responsive Styling */
@media (max-width: 480px) {
  .whatsapp-float {
    width: 54px;
    height: 54px;
    bottom: 18px;
    right: 18px;
  }

  .whatsapp-float svg {
    width: 28px;
    height: 28px;
  }
}
```

## 🖥️ WordPress Integration

If your website uses WordPress or WooCommerce, you can integrate the button manually or use a plugin.

1. Log in to your WordPress dashboard.
2. Navigate to **Plugins → Add New Plugin**.
3. Search for a WhatsApp chat plugin, such as Joinchat.
4. Install and activate the plugin.
5. Configure your WhatsApp phone number and greeting message.

Avoid enabling both the manual button and a plugin-generated button simultaneously, as this may display duplicate buttons.

## ✅ Testing Checklist

- [ ] The WhatsApp button appears in the bottom-right corner.
- [ ] The button remains visible when scrolling.
- [ ] Clicking the button opens WhatsApp.
- [ ] The correct business phone number is displayed.
- [ ] The pre-filled message appears correctly.
- [ ] The layout works on desktop and mobile devices.
- [ ] The button supports keyboard navigation.
- [ ] The Live Demo badge opens the deployed website.

## 🎨 Customization

| Property | Description |
|---|---|
| Phone number | Set your WhatsApp number in international format. |
| Message | Change the URL-encoded pre-filled message. |
| `background-color` | Change the button background color. |
| `width` and `height` | Adjust the button size. |
| `bottom` and `right` | Change the button position. |
| `border-radius` | Adjust the button shape. |

## 📄 License

This project is available for personal and commercial use. You may modify and integrate the code into your own website.

---

**Live Website:** [shawebdesign.com](https://shawebdesign.com/)

**Project:** Floating WhatsApp Chat Button

**Purpose:** Make it easy for website visitors to contact a business directly through WhatsApp.
