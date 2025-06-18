# 🕵️‍♂️ Steganography – Hiding Information in the Image

This project demonstrates a simple yet effective image steganography technique using **Least Significant Bit (LSB)** manipulation. It allows users to hide and extract secret messages within image files without visibly altering the image. Ideal for secure and invisible communication.

---

## 🧠 Problem Statement

In today's digital world, hiding sensitive information securely has become a major challenge. While encryption secures the data, its presence is still noticeable. **Steganography** goes one step further by hiding the existence of the message itself. This project implements LSB-based steganography to invisibly embed text into images.

---

## 🛠️ System Development Approach

- **Programming Language:** Python
- **Libraries Used:**
  - `Pillow` – Image processing
  - `NumPy` – Efficient pixel manipulation
- **Input:** Cover image (PNG/JPEG), Secret message
- **Output:** Image with embedded message or extracted secret text

---

## ⚙️ Algorithm & Deployment

### 🔐 Hiding Message:
1. Convert each character of the secret message into binary.
2. Append a unique delimiter (`####`) to mark the end.
3. Modify the Least Significant Bit of each image pixel to match the message bits.
4. Save the new stego image.

### 🔓 Extracting Message:
1. Read the LSBs from the stego image.
2. Group every 8 bits and convert to ASCII characters.
3. Stop reading when the delimiter `####` is detected.
4. Output the hidden message.

---

## ✅ Result

- The output image looks visually identical to the original.
- The hidden message can only be extracted using this script.
- Message capacity depends on image size.

> ✅ Works best with 256×256 PNG images  
> ✅ Preserves the quality and integrity of the original image

---

## 📷 Example Output

> 💬 Hidden Message: `"Confidential Data: Project X"`  
> 📁 Output File: `stego_image.png`

---

## 📌 Conclusion

This project provides a lightweight and effective method for hiding sensitive text within images using LSB steganography. It showcases how steganographic techniques can add a layer of confidentiality on top of encryption. While simple, it forms the basis for more advanced and secure hiding methods.

---

## 🔮 Future Scope

- Add support for audio or video steganography.
- Encrypt the message before embedding.
- Build a GUI with Tkinter or a web interface using Flask.
- Use deep learning for adaptive steganography.

---

## 📚 References

- [Wikipedia – Steganography](https://en.wikipedia.org/wiki/Steganography)
- [Pillow Documentation](https://pillow.readthedocs.io/)
- Research Paper: “A Review on Image Steganography Techniques” – [IEEE Xplore](https://ieeexplore.ieee.org/document/9043720)

---


---

## 🧑‍💻 Author

**Mayank Saini**  
_Computer Science & Engineering, [Rajkiya Engineering College Kannauj]_

