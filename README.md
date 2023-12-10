# Scalable-Machine-Learning-Lab_2

Text Transcription using Transformers to your Mother Tongue.

## Improvements

- model-centric approaches:

1.  tune hyperparameter - set `warmup_steps=100` and `max_steps=1000`. We found that the model starts overfitting after 1000 epochs.
2.  change model - use `openai/whisper-medium` instead of `openai/whisper-small`. We found the eval loss stop decreasing after 1000 epochs which means the performance ceiling of small model has been reached.

- data-centric approach: Increase sampling rate to 24000 to get more details.

App URL: https://huggingface.co/spaces/esnagy/hungarian_speech_transcriber
