# SimpleSynth

A web-based synthesizer built with React and the Web Audio API. Create and manipulate sounds in real-time with an intuitive interface.

## Features

- **Real-time Sound Generation**: Generate tones using multiple oscillators with adjustable harmonics
- **Interactive Controls**:
  - Frequency range: 20 Hz - 20 kHz (logarithmic scale)
  - Volume control (0-100%)
  - Harmonic complexity (1-9 harmonics)
  - Reverb effect (0-100%)
- **Visual Feedback**: Real-time waveform visualization on canvas
- **Easy Controls**: Play/Stop and Randomize buttons for quick experimentation
- **Responsive Design**: Works on desktop and mobile devices

## How to Use

1. Open `index.html` in any modern web browser
2. Click "Play" to start generating sound
3. Adjust the sliders to modify:
   - **Frequency**: Changes the base pitch
   - **Volume**: Controls overall loudness
   - **Harmonics**: Adds overtones for richer sounds
   - **Reverb**: Adds spatial depth
4. Use "Randomize" to generate new parameter combinations
5. Click "Stop" to silence the synthesizer

## Technologies

- **React**: UI framework for component-based interface
- **Web Audio API**: Browser-native audio processing
- **Tailwind CSS**: Utility-first CSS framework for styling
- **Babel**: JavaScript transpilation for JSX support
- **Lucide**: Icon library for UI elements

## Browser Compatibility

Works in all modern browsers that support the Web Audio API:

- Chrome 14+
- Firefox 25+
- Safari 6+
- Edge 12+

## Architecture

The synthesizer uses a modular audio graph:

```
Oscillators → Gain Node → Dry/Wet Split → Reverb → Output
```

- Multiple oscillators create harmonic content
- Convolution reverb provides spatial effects
- Real-time parameter updates without audio glitches

## Development

This is a standalone HTML file with no build process required. All dependencies are loaded via CDN for easy deployment and offline use.

## License

MIT License - feel free to use and modify as needed.
