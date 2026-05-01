# 04 — System Architecture

## Layers

### Layer 1 — Input
- Uploaded audio file (.wav, .mp3)
- Microphone recording
- Pre-recorded campus audio clips

### Layer 2 — Processing
- librosa loads audio at 22050 Hz
- Convert to Mel-spectrogram (128 mel bands)
- Normalise and resize to 128x128 pixels
- Apply augmentation during training

### Layer 3 — Intelligence (CNN)
- Input: 128x128 spectrogram image
- Conv2D → ReLU → MaxPool (x3)
- Dropout (0.3)
- Fully Connected → Softmax
- Output 1: Genre (10 classes)
- Output 2: Mood (4 classes — mapped from genre)
- Output 3: Wellness score (for noise map)

### Layer 4 — Application
- Health module: 7-day genre shift tracker → alert
- Social module: Folium noise heatmap
- Gradio UI: upload → classify → display results

## Data Flow
Audio Input → Mel Spectrogram → CNN → 
Genre + Mood → Health Alert / Noise Map → User
