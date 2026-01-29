# MuseGAN: AI-Powered Music Generation

A deep learning project that implements MuseGAN (Multi-track Sequential Generative Adversarial Networks) for automatic music composition. This project trains a GAN model from scratch to generate multi-track music pieces using PyTorch.

## Overview

This project explores the fascinating intersection of artificial intelligence and music composition. By leveraging Generative Adversarial Networks (GANs), the model learns to create original music pieces that follow musical theory principles including chords, melody, groove, and style.

## Features

- **Music Theory Foundation**: Understanding of musical notes, octaves, and pitch
- **Multi-track Generation**: Creates music with multiple instrumental tracks
- **Piano Roll Representation**: Digital representation of music for neural network processing
- **Custom GAN Architecture**: Implements both Generator and Critic (Discriminator) networks
- **MIDI Processing**: Converts generated tensors to playable MIDI files
- **Audio Synthesis**: Transforms MIDI to audio using FluidSynth

## Project Structure

```
Muse-GAN/
├── MuseGAN.ipynb          # Main Jupyter notebook with complete implementation
├── README.md              # Project documentation
├── requirements.txt       # Python dependencies
└── LICENSE               # MIT License
```

## What's Inside the Notebook

The `MuseGAN.ipynb` notebook contains a comprehensive tutorial covering:

1. **Digital Music Representation**
   - Musical notes, octaves, and pitch numbers
   - Introduction to multi-track music
   - Piano roll digital representation

2. **Music Generation Blueprint**
   - Constructing music with chords, style, melody, and groove
   - MuseGAN architecture design

3. **Data Preparation**
   - Downloading and loading training datasets
   - Converting multidimensional objects to music pieces

4. **MuseGAN Architecture**
   - Critic (Discriminator) network implementation
   - Generator network implementation
   - Optimizers and loss functions

5. **Training**
   - Training loop implementation
   - Gradient penalty for stable training

6. **Music Generation**
   - Generating new music with the trained model
   - Results analysis and visualization

## Requirements

- Python 3.7+
- PyTorch
- music21
- numpy
- matplotlib
- midi2audio (FluidSynth)
- IPython

See `requirements.txt` for specific versions.

## Installation

1. Clone this repository:
```bash
git clone https://github.com/yourusername/Muse-GAN.git
cd Muse-GAN
```

2. Install the required dependencies:
```bash
pip install -r requirements.txt
```

3. Install FluidSynth (for audio synthesis):
   - **Ubuntu/Debian**: `sudo apt-get install fluidsynth`
   - **macOS**: `brew install fluid-synth`
   - **Windows**: Download from [FluidSynth website](https://www.fluidsynth.org/)

## Usage

1. Open the Jupyter notebook:
```bash
jupyter notebook MuseGAN.ipynb
```

2. Run the cells sequentially to:
   - Learn about music theory fundamentals
   - Prepare the training data
   - Build the MuseGAN architecture
   - Train the model
   - Generate new music pieces

3. The notebook will guide you through each step with detailed explanations and visualizations.

## How It Works

MuseGAN uses a sophisticated architecture that separates music generation into different components:

- **Chords Track**: Generates the harmonic structure
- **Style Track**: Defines the overall musical style
- **Melody Tracks**: Creates individual melodic lines for different instruments
- **Groove Track**: Establishes rhythmic patterns

The model learns from existing music pieces represented as 4D tensors (tracks × bars × time steps × pitches) and generates new compositions following similar patterns.

## Model Architecture

- **Generator**: Transforms random noise into realistic music sequences
- **Critic**: Evaluates generated music and provides feedback to improve generation
- **Loss Function**: Wasserstein loss with gradient penalty for stable training

## Results

The trained model can generate:
- Multi-track music pieces
- Coherent chord progressions
- Melodic variations
- Rhythmic patterns

Generated pieces can be exported as MIDI files and converted to audio for playback.

## Technologies Used

- **PyTorch**: Deep learning framework
- **music21**: Music analysis and generation toolkit
- **NumPy**: Numerical computing
- **Matplotlib**: Visualization
- **FluidSynth**: MIDI to audio conversion

## Learning Outcomes

This project demonstrates:
- Implementation of GANs from scratch
- Music theory application in AI
- Data preprocessing for creative AI tasks
- Working with MIDI and audio formats
- Training techniques for stable GAN convergence

## Future Improvements

Potential enhancements:
- Implement different music styles
- Add user controls for generation parameters
- Extend to longer compositions
- Incorporate transformer architectures
- Add real-time generation capabilities
- Web interface for easy interaction

## References

- [MuseGAN Paper](https://arxiv.org/abs/1709.06298) - Original MuseGAN research
- [PyTorch Documentation](https://pytorch.org/docs/)
- [music21 Documentation](https://web.mit.edu/music21/)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

## Acknowledgments

- Original MuseGAN paper by Hao-Wen Dong, Wen-Yi Hsiao, Li-Chia Yang, and Yi-Hsuan Yang
- PyTorch community for excellent deep learning tools
- music21 community for music processing utilities

## Contact

Feel free to reach out if you have any questions or suggestions!

---

**Note**: This is an educational project demonstrating the capabilities of GANs in creative domains. Generated music quality depends on training data quality and quantity.
