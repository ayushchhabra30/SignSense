# 🤟 SignSense: Talking with Your Hands, Literally!

> An AI-powered magic mirror that translates hand gestures into text in real-time. We mashed up static and motion recognition so you can sign full sentences on the fly!

---

## 📌 What's the Big Idea?

Ever wished your webcam could understand sign language? Meet **SignSense**! We built a real-time translator that watches your hands and types out what you're saying. It uses a "hybrid" AI brain:

- **Static mode:** For the ABCs, 123s, and spaces (striking a pose!).

- **Motion mode:** For whole words that require movement (action!).

Using some slick hand-tracking tech, we made it fast, interactive, and ready to help break down communication barriers.

---

## ✨ The Cool Stuff

- ⚡ **Blink-and-you-miss-it Translation:** Real-time gesture-to-text conversion.

- 🧠 **Double-Brained AI:** Hybrid model combining Static + Motion recognition.

- 📝 **Sentence Builder:** Strings your predicted gestures together into actual sentences.

- 🔀 **Shape-Shifting Modes:** Easily toggle between static and motion detection.

- ⌨️ **Oops-Proof Controls:** Interactive commands to clear, backspace, or delete a word when you fumble.

---

## 🛠️ Our Geeky Toolbox

| Tool | Superpower |

|------|------------|

| Python | The trusty glue holding it all together |

| OpenCV | The eyes of the operation (Video capture & processing) |

| MediaPipe | The skeletal mapper (Tracking those hand landmarks) |

| Scikit-learn (Random Forest) | The static shape spotter |

| TensorFlow / Keras (LSTM) | The motion pattern psychic |

| NumPy | The ultimate number-crunching ninja |

---

## ⚙️ Under the Hood

### 🟢 Striking a Pose (Static Gesture Recognition)

- MediaPipe grabs **21 key points** on your hand.

- We crunch those into **42 normalized features** (x, y coordinates).

- Our **Random Forest classifier** plays a lightning-fast game of "guess the letter/number."

### 🔵 Action Sequence (Motion Gesture Recognition)

- We capture mini-movies of **30 frames**.

- Each frame packs those same **42 features**.

- Our **LSTM model** watches the flow to predict dynamic, moving words. It's all about that temporal rhythm!

### 🟣 The Ultimate Mashup (Hybrid System)

- We jammed both brains into a **single smooth pipeline**.

- Manual mode switching keeps the AI from getting confused.

- The final outputs are stitched together to form **meaningful sentences**.

## 🦸‍♂️ Our Super-Suit Upgrades (What we Did)

- Architected the **landmark-based feature extraction pipeline** (wrangling those 42 features per frame).

- Trained the **Random Forest** model for static gestures.

- Built the **LSTM-based sequence model** for motion gestures.

- Engineered the **hybrid inference pipeline** to make both models play nice together.

- Crunched the evaluation metrics to prove it actually works.

- Got my hands dirty creating and prepping the **dataset**.

---

---

## 🚧 Roadblocks & Next Levels

**Current Glitches in the Matrix:**

- We speak ASL right now because ISL datasets are hard to find.

- Moody lighting and different users can sometimes confuse the AI.

**Level Up (Future Work):**

- [ ] Learn Indian Sign Language (ISL) 🇮🇳

- [ ] Beef up the dataset (More hands, more backgrounds!) 📸

- [ ] Take it to the web (Web app incoming!) 🌐

---

---

## 🚀 DIY Time (How to Run)

```bash

# Clone the repository to your machine

git clone https://github.com/shivanshh-oo/SignSense.git

# Jump into the project folder

cd Signsense-main

# Install all the necessary robot brains

pip install opencv-python mediapipe scikit-learn tensorflow numpy jupyter pyttsx3

# Fire it up!

click *run all* Hybrid_inference_classifier.ipynb file 
