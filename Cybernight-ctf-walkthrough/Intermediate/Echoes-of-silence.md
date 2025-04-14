# Cyber Night CTF Day 01 Walkthrough Challenge 2


**Description:**

The hidden message lies within the frequencies of the audio. Start by examining the spectral data of the .wav file, and listen closely for any patterns or anomalies that might reveal something hidden in plain sight. Could subtle changes in the waves be the key to unlocking the truth?

**Level**: Intermediate  🟡 <br>
**Challenge Link**:[Echoes of silence](https://t.me/AASTU_CyberClub/151) <br>
**Technique**: Audio Spectrogram Steganography (Text-based)  <br>
**Tool**: [Sonic Visualizer](https://www.sonicvisualiser.org/) <br>
**Point: 200** <br>


### Concept Behind the Challenge

#### 🎵 What Is Spectrogram-Based Steganography?

A **spectrogram** is a visual representation of sound: frequency (vertical) over time (horizontal), with brightness indicating intensity.

In this challenge, a **text flag** (like `flag{text_flag}`) was **rendered as an image**, and that image was **converted into sound waves**. When opened with a spectrogram viewer, the hidden message is revealed visually — **not audibly**

https://github.com/user-attachments/assets/d90988f90165bf4746a0c08314bc534ab2da4f47


Boom we got the flag for challenge two but it is inverted, so we need to take screenshot and flip it Vertically then flip Horizontally. Here we goooo we found our flag.

![flag1](https://github.com/0xfke/0xfke.github.io/blob/313b7687cd472af4ee5622c018a9bf1f793a443b/Images/WriteUp-Image/flag1.png)

✅ **Flag captured successfully!**

```sh
flag{audio_wav3s_n3v3r_1i3}
```

Steganography in audio files is crucial for both **Red Team** operations, where it hides payloads or C2 data to evade detection, and **Blue Team** defense, where identifying covert channels is vital during DFIR. For **CTF competitors**, it enhances **analytical skills** and **creative problem-solving**. This technique is often used in **APT operations** and **C2 channels** to bypass traditional security measures. The challenge teaches **visual steganography** in audio, **tool-based investigation**, **pattern recognition**, and exposes participants to **real-world adversarial techniques**.

**Room by**: [0xfke](https://0xfke.github.io/about)
