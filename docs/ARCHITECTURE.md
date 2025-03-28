# Architecture Overview

## Core Components
- **UI Layer**: Jetpack Compose components
- **Business Logic**: Model generation pipeline
- **Machine Learning**: TensorFlow Lite integration
- **3D Rendering**: Filament engine

## Key Features
- Image-to-3D conversion pipeline
- Interactive 3D visualization
- Asynchronous processing
- Clean state management

## Data Flow
1. User selects image
2. System converts to bitmap
3. GET3D model processes image
4. 3D data sent to viewer
5. User interacts with 3D model

## Technical Stack
- Kotlin
- Jetpack Compose
- TensorFlow Lite 2.7+
- Filament 1.20+
- Android SDK 24+