
# 🧾 QR Code Generator in Python (with GUI) – 2025 Tutorial

## 🔗 Watch the Video Tutorial
🎥 [Click here to watch on YouTube](https://www.youtube.com/watch?v=P4YGMhUOeKg)

---

## 🐍 What You’ll Build

In this tutorial, you’ll learn how to create a **QR Code Generator** using Python. You’ll start with a basic script and then level up by adding a **Graphical User Interface (GUI)** using `Tkinter`. You can even customize the **colors** and **embed logos** into your QR codes!

---

## 📦 Requirements

Install the required packages:

```bash
pip install qrcode[pil] pillow
```

---

## 📄 Basic QR Code Generator (CLI)

```python
import qrcode

# Text or URL to encode
data = input("Enter the text or URL to encode in QR code: ")

# Generate QR Code
qr = qrcode.QRCode(
    version=1,
    error_correction=qrcode.constants.ERROR_CORRECT_H,
    box_size=10,
    border=4,
)
qr.add_data(data)
qr.make(fit=True)

# Create the image
img = qr.make_image(fill_color="black", back_color="white")

# Save the image
img.save("my_qr_code.png")
print("✅ QR Code generated and saved as my_qr_code.png")
```

Quick version:
```python
data = "https://geekyscript.com"
img = qrcode.make(data)
img.save("quick_qr.png")
```

---

## 🎨 Bonus: QR Code Generator with GUI (Tkinter)

This GUI app lets users:
- Input text or URLs
- Choose fill and background colors
- Add a custom logo in the center of the QR Code
- Save the generated QR image

```python
# Full GUI code here...
# (Refer to script provided above in your environment)
```

### Screenshot:
> Include a screenshot of your GUI app if you're uploading this to GitHub or a blog.

---

## 💾 Features

- ✅ Custom text/URL input
- 🎨 Choose fill and background colors
- 🖼️ Add a logo/image
- 💾 Save QR as PNG

---

## 🧠 Fun Ideas

- Generate QR for business cards
- Use it in event badges
- Share WiFi credentials
- Add QR codes to product packaging

---

## 🔗 YouTube Video Link

📺 [Watch the Full Tutorial on YouTube](https://www.youtube.com/watch?v=P4YGMhUOeKg)

---

## 🙌 Happy Coding!

Let us know what you create by tagging [@YourChannelName] on social media!
