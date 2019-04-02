# Street-Fighter-II-AI-Voice-Control

Street Figher II (Genesis) on Raspberry Pi 3B, with AI and voice control for game play.

AI is used for basic movements, and voice recognition is used for special movements. For example: you can say "Hadouken" to trigger Ryu's Hadouken movement in game.

The AI is trained with Deep Reinforcement Learning on an AWS server, then the model is used for game play on Raspberry Pi. Two algorithms: DQN and DDPG have been tested and both are working. Both raw pixels and human-designed features can be used for training. To reduce the reqirement for computing power, which is limited on Raspberry Pi, human-designed features are preferred for this project.

The voice control is implemented with LD3320, which is a ASR Speaker-Independent Automatic Speech Recognition Module with a SPI interface.

The system is based on Pi64 image (64bit Debian Stretch), and most code is written in Python.
