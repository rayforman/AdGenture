# 🎮 AdGenture

<img src="/public/example-image.png" alt="AdGenture Example" width="50%"/>

A generative interactive adventure game that combines text-based storytelling with AI-generated visuals. AdGenture uses advanced machine learning models to create a unique gaming experience where your choices shape both the narrative and the visual elements of your journey. The best part? No two stories are the same! And due to its generative nature, there are literally infinite possible games.

## ✨ Features

* Dynamic story generation based on user choices
* AI-powered image generation for each scene
* Interactive GUI built with Python's tkinter
* Five-round adventure format with multiple endings
* Custom sprite generation using advanced pixelization techniques

## 🛠️ Technical Stack

* **Frontend**: Python tkinter for GUI
* **Image Generation**: Modified Wuerstchen model
* **Sprite Creation**: Aliasing-Aware Pixelization
* **GPU Support**: Single GPU optimization (modified from DDP)

## 🚀 Getting Started

### Prerequisites

* Python 3.8+
* CUDA-compatible GPU
* Required Python packages (see `requirements.txt`)

### Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/adgenture.git
cd adgenture
```

2. Download model weights:
   * Access the weights from our [Google Drive](https://drive.google.com/drive/folders/1oTVD4C_WoJrBuP23Y0F6lhIIdpZSkObc?usp=sharing)
   * Place both weight files in the `./weights/` directory

3. Install dependencies:
```bash
pip install -r requirements.txt
```

### Running the Game

Launch the application:
```bash
python app.py
```

## 🎯 How to Play

1. Launch the application
2. Click the button to select your seed text
3. Read the story and view the generated image
4. Choose your next action from the available options
5. Continue for five rounds until reaching a conclusion

## 🔧 Architecture

The project combines multiple AI models and systems:

* **Story Generation**: Custom text generation pipeline
* **Image Creation**: Modified Wuerstchen model for scene generation
* **Sprite System**: Aliasing-Aware and Cell-Controllable Pixelization

## 🙏 Acknowledgments

This project builds upon and uses code from:

* [Make Your Own Sprites: Aliasing-Aware and Cell-Controllable Pixelization](https://github.com/WuZongWei6/Pixelization) - For sprite generation
* [Wuerstchen](https://github.com/dome272/Wuerstchen) - Modified for single GPU support and custom dataset integration

### Key Modifications

* Adapted Wuerstchen's Stage C Training Loop from DDP to Single GPU
* Implemented custom dataset support
* Enhanced inference pipeline for real-time generation

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

## 📬 Contact

For questions and support, please open an issue in the GitHub repository.

---

Made with ❤️ by Ray Forman, Ethan Chang, Alessandro Castillo, and Stephen Pasch