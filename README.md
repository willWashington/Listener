# Listener
Listener is a part of a larger Windows Worker Service infrastructure designed like a microservices application. Listener plays the part of listening to internal system audio, translating that audio into a parsable set of data, and sending that data to Azure for SpeechConigition services. 

## Goal:
The goal of this worker service is to be able to capture phrases of interest from a stream of live audio and collect the things that were said about them. My current implementation is part of a larger Stock market app that I am designing that will capture Stock Market tickers and plays from a live audio stream, provide me recent news and stock trends (hopefully sentiment if I can manage that level of intelligence), and suggest whether or not the ticker is bullish or bearish based on various market formulas. Because the goal is to consume audio and research a company based off the audio, the Listener sub-service is foundational to the entire application.
