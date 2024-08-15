# Augmented Reality App Using ARKit - README

## 1. Goal
The primary goal of this project is to create an augmented reality (AR) app using ARKit in Swift that displays 3D models of Captain America and Iron Man when their respective playing cards are detected. The app leverages image recognition technology within ARKit to detect custom markers (playing cards), triggering the display of corresponding superhero 3D models.

## 2. Process
### 2.1. Tools and Frameworks
ARKit: Apple's AR framework for detecting images and placing virtual objects in real-world scenes.\
SceneKit: Used for rendering and displaying 3D models within the AR experience.\
Swift: Programming language used to build the iOS app.
### 2.2. Steps
#### Set Up the AR Session:

Initialize an AR session with ARImageTrackingConfiguration to track specific images.
Define a reference image set that includes the playing cards of Captain America and Iron Man, each associated with a corresponding image.

#### Adding Reference Images:

The playing card images are added to an AR Resource Group in the Xcode project.\
The images are referenced in the AR session configuration to detect them during runtime.

#### Loading 3D Models:

3D models of Captain America and Iron Man are created or downloaded in .dae or .usdz format and added to the project.\
SceneKit is used to load these models and handle their rendering.

#### Implementing Image Detection:

ARKit's ARImageAnchor is utilized to detect when one of the playing cards is recognized in the camera view.\
When a match is found, the app displays the appropriate 3D model anchored to the location of the detected card.

#### Animating and Interacting with 3D Models:

Basic animations or interactivity (e.g., rotating the models) are implemented using SceneKit.\
Touch gestures can be added to interact with the displayed models.

#### Running the AR Experience:

The app runs an AR session, continuously scanning for the playing cards and updating the AR scene when a card is detected.

### 2.3. Code Structure
#### ViewController.swift: Contains the main AR session logic, including the setup for image detection and loading of 3D models.
#### Assets.xcassets: Stores the reference images for the playing cards and the 3D models.
#### AR Resources: Contains the custom reference image set used for image detection.

## 3. Result
The final AR app allows users to experience an interactive scene where the 3D models of Captain America and Iron Man are displayed when their respective playing cards are recognized. When a card is detected, the relevant 3D model appears in the real-world environment, anchored to the card's position. This project demonstrates how ARKit can be used for image recognition and immersive AR experiences, combining custom 3D content with real-world triggers.

### Key Features:
Accurate image detection for triggering 3D models.\
Seamless integration of 3D content with real-world objects.
