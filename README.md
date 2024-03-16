# EPOCH_PS1_mithu
Multilingual unit to WAV vocoder 


# VITS: Multilingual Text-to-Speech (TTS) Model
## Overview
VITS (Variational Inference with adversarial learning for end-to-end Text-to-Speech) is an *end-to-end speech synthesis model* that predicts a speech waveform based on an input text sequence. It is a *conditional variational autoencoder (VAE)*, consisting of the following components:

1. *Posterior Encoder*: Encodes input text into latent representations.
2. *Decoder*: Generates spectrogram-based acoustic features.
3. *Conditional Prior*: Provides additional context for waveform synthesis.

The model also includes a *stochastic duration predictor, allowing it to synthesize speech with different rhythms from the same input text. VITS is trained end-to-end using a combination of variational lower bound and adversarial training. To enhance expressiveness, **normalizing flows* are applied to the conditional prior distribution.

## Model Details
- *Architecture*: VAE with flow-based module
- *Text Encoding*: Transformer-based text encoder
- *Waveform Synthesis*: HiFi-GAN decoder
- *Language Support*: English (hin) language TTS model
- *Non-Deterministic*: Requires a fixed seed for consistent speech waveform generation

2. Save the resulting waveform as a .wav file using your preferred audio library.

## Acknowledgments
This model is part of Facebook's *Massively Multilingual Speech (MMS)* project, aiming to provide speech technology across a diverse range of languages. 

## License
This model is available under the *CC-BY-NC-4.0* license.

---
