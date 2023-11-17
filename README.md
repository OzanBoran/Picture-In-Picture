# Picture-in-Picture JavaScript Project

This project demonstrates the usage of the Picture-in-Picture API in a web application. When the user clicks the "START" button, the video enters Picture-in-Picture mode, allowing it to be displayed in a floating window over other applications or windows.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [JavaScript Methods](#javascript-methods)
- [Deployment](#deployment)
  
## Features

- Implements Picture-in-Picture functionality using the Web API.
- Styled user interface with a custom button.
- Responsive design for various screen sizes.

## Installation

Clone the repository to your local machine using Git:

```bash
git clone https://github.com/OzanBoran/Picture-In-Picture
```

Change into the project directory:
cd Picture-In-Picture

Open index.html in your preferred web browser.

## Usage

1. Open the `index.html` file in your web browser.
2. Click the "START" button to enable Picture-in-Picture mode.
3. Resize and move the floating video player as needed.
4. Click the Picture-in-Picture window to return to normal mode.

## JavaScript Methods

### `navigator.mediaDevices.getDisplayMedia()`

This method prompts the user to select a media stream (in this case, the screen or a specific application window) and returns a `MediaStream` object.

### `videoElement.srcObject = mediaStream;`

This assigns the obtained `MediaStream` object to the `srcObject` property of the `videoElement`, effectively setting up the video source.

### `videoElement.onloadedmetadata = () => { videoElement.play(); };`

This event listener ensures that the video starts playing once the metadata (such as duration and dimensions) is loaded.

### `videoElement.requestPictureInPicture()`

This method is called when the user clicks the "START" button. It requests to enter Picture-in-Picture mode for the video element, allowing it to float over other content.

### Error Handling

In the JavaScript code, errors are caught using a `try-catch` block. If there are any errors during the attempt to enter Picture-in-Picture mode, they will be logged to the console for further debugging.

## Deployment

The project is deployed and can be accessed online at: https://ozanboran.github.io/Light-Dark-Mode/

## Credits
- **Developer:** Ozan Boran
