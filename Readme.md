# ChatGPT Molly-guard Chrome Extension

## Overview
ChatGPT Molly-guard is a Chrome extension that acts as a protective layer when interacting with ChatGPT. It prevents accidental submission of sensitive information by monitoring the chat input for specified words or phrases.

The term "molly-guard" traditionally refers to a protective cover over a button to prevent accidental activation. In this context, it serves as a digital guardian against inadvertent sharing of sensitive information.

## Features
- Real-time monitoring of chat input
- Visual feedback when sensitive words are detected (red border and background)
- Automatic disabling of the submit button when forbidden words are present
- Case-insensitive word matching
- Prevention of both button clicks and Enter key submissions

## Technical Implementation
The extension is built using standard web technologies:
- **manifest.json**: Defines the extension configuration and permissions
- **contentScript.js**: Handles the core functionality of monitoring and UI manipulation
- **wordList.js**: Contains the configurable list of forbidden words
- **style.css**: Provides visual feedback styling

### Key Components
1. **Content Script**: Implements debounced input monitoring and UI updates
2. **Word Detection**: Case-insensitive matching against a predefined list
3. **UI Feedback**: Visual indicators when sensitive content is detected
4. **Event Handling**: Manages both keyboard and mouse interactions

## Installation
Currently under review in the Chrome Web Store. For development:

1. Clone this repository
2. Open Chrome and navigate to `chrome://extensions/`
3. Enable "Developer mode"
4. Click "Load unpacked" and select the extension directory

## Learning Outcomes
This project demonstrates several key concepts in Chrome extension development:
- Content script implementation and DOM manipulation
- Event handling in Chrome extensions
- Manifest V3 structure and configuration
- Cross-page JavaScript injection
- UI/UX considerations for user feedback

## Future Improvements
- Add user interface for dynamic word list management
- Implement paste event handling
- Add contextual override capabilities
- Expand matching patterns beyond simple word matching

## Credits
Based on the tutorial from [SitePoint](https://www.sitepoint.com/create-chrome-extension-10-minutes-flat/)

## License
MIT License

Copyright (c) 2024

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
