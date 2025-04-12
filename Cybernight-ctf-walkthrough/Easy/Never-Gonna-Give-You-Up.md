# Walkthrough – Challenge 1: *Hidden in Plain Sight*

**Level**: Easy 🟢
**Technique**:  EXIF-based Steganography
**Tool**: [Exiftool](https://github.com/exiftool/exiftool)
### Concept Behind the Challenge

#### 💡 What Is EXIF-based Steganography?

EXIF (Exchangeable Image File Format) is a standard for storing metadata in image files, such as camera details, GPS coordinates, date, and other properties. **EXIF-based steganography** involves hiding information, such as a flag, within this metadata, which is invisible in the image itself but can be extracted with tools like **ExifTool**.

In this challenge, the **flag** is hidden inside the **metadata of an image** file. The key to discovering it lies in extracting and analyzing the **EXIF metadata** of the image file.

#### 🌐 OSINT Relevance:

EXIF metadata is often **overlooked in publicly posted files** on social media, blogs, or websites. Attackers may use EXIF-based steganography to embed covert messages in **images** shared online, making it harder to detect at first glance. For **OSINT (Open-Source Intelligence)** gathering, analyzing metadata from publicly available images can provide critical information — from hidden messages to **location data** or even **timestamps** that reveal more about a target.

![[Pasted image 20250412003402.png]]

This string looks like it is encrypted using base64 from the structure at the end "=". taking it and decoding it gives us our first flag.

![[Pasted image 20250412003630.png]]


You can also take the encrypted string and go to [cyberchef](https://gchq.github.io/CyberChef/) web which is basically a decryption and encryption tools repo.
![[20250411-2140-49.0223627.mp4]]

✅ **Flag captured successfully!**


```sh
flag{h3110_fr0m_th3_0th3r_1ay3r}
```
