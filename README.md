# Dinosaur AR Filters

This repository contains two Augmented Reality (AR) filters for Instagram, featuring interactive 3D dinosaur models. Each filter includes functionalities to switch between different dinosaurs and play synchronized dinosaur roars.

## Table of Contents

- [Features](#features)
- [Folder Structure](#folder-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Development](#development)
- [Contributing](#contributing)
- [License](#license)

## Features

- Interactive 3D dinosaur models.
- Optimized 3D models with reduced triangle count for better performance.
- Audio integration with synchronized dinosaur roars.
- Button-based picker to switch between different dinosaurs.
- Information button to display details about each dinosaur.

## Folder Structure

```plaintext
dinosaur-ar-filters/
│
├── dino1/
│   ├── objects/
│   │   ├── fliyingdino/
|   |   |   ├── flyingdino.glg
|   |   ├──tyranno/
│   │   |   ├── tyranno.glb
|   |   ├──velocrip/
│   │   |   ├── velocrip.glb
│   ├── audios/
│   │   ├── audio1.audioctrl
│   │   ├── audioflying.audioctrl
│   │   └── audiorunning.audioctrl
│   └── dino1.arproj
│
├── dino2/
│   ├── objects/
│   │   ├── meshtrex.glb
│   ├── audio/
│   │   ├── audioroar.audioctrl
│   │   ├── audiorunning.audioctrl
│   │   ├── audiotail.audioctrl
│   └── dino2.arproj
│
└── README.md
```

## Installation

### Prerequisites
- Meta Spark Studio installed.
- Blender for 3D model editing.
- Meta Spark Player for Testing your filters
- Basic knowledge of AR filter creation and 3D modeling.

### Steps

1. **Clone the repository**:

    ```bash
    git clone https://github.com/devprashad/dinosaur-ar-filters.git
    ```

2. **Open Meta Spark Studio**:

    - Ensure Meta Spark Studio is installed on your system.
    - Open the Meta Spark Studio application.

3. **Load the project**:

    - Within Meta Spark Studio, load the project for the desired filter (`dino1` or `dino2`).

4. **Import Assets**:

    - Navigate to the folder of the chosen filter (`dino1` or `dino2`) and open the `dino1.arproj` or `dino2.arproj` .
    - Import the 3D models (GLB format) and audio files into Meta Spark Studio as needed.

5. **Configure Project**:

    - Set up trackers (plane) as required for your AR experience.
    - Use the Patch Editor to add interaction logic for switching dinosaurs and displaying information.

6. **Test with Meta Spark Player**:

    - Download and install [Meta Spark Player](https://sparkar.facebook.com/ar-studio/learn/spark-ar-player) from the Google Play Store or Apple App Store.
    - Export your project to test the AR filter using Meta Spark Player.

7. **Export**:

    - Once satisfied with the filter, export the project for use on Instagram.

   
## Usage

### Using Dino1 Filter

1. **Open the Project in Meta Spark Studio**:

    - Navigate to `dino1` and open `dino1.arproj`.

2. **Import Assets**:

    - Ensure all 3D models (GLB format) and audio files are properly imported.

3. **Add Trackers**:

    - Add plane, or other trackers as required for your AR experience.

4. **Setup Buttons and Interaction**:

    - Use the Patch Editor to add interaction logic for switching dinosaurs and displaying information.

5. **Test with Meta Spark Player**:

    - Download and install Meta Spark Player from the Google Play Store or Apple App Store.
    - Export your project to test the AR filter using Meta Spark Player.

6. **Export**:

    - Once satisfied, export the filter for use on Instagram.

### Using Dino2 Filter

1. **Open the Project in Meta Spark Studio**:

    - Navigate to `dino2` and open `dino2.arproj`.

2. **Import Assets**:

    - Ensure all 3D models (GLB format) and audio files are properly imported.

3. **Add Trackers**:

    - Add face, plane, or other trackers as required for your AR experience.

4. **Setup Buttons and Interaction**:

    - Use the Patch Editor to add interaction logic for switching dinosaurs and displaying information.

5. **Test with Meta Spark Player**:

    - Download and install Meta Spark Player from the Google Play Store or Apple App Store.
    - Export your project to test the AR filter using Meta Spark Player.

6. **Export**:

    - Once satisfied, export the filter for use on Instagram.


## Development 
### Reducing Triangles in Blender

1. **Open the Model**:
   - Open Blender and load your dinosaur model.
2. **Decimate Modifier**:
   - Apply the Decimate Modifier to reduce the number of triangles in the model.
   - Aim to optimize the model to have around 50,000 triangles for optimal performance in AR applications.
3. **Export the Model**:
   - Export the optimized model in GLB format for use in Meta Spark Studio.

### Setting Up in Meta Spark Studio

1. **Import Optimized Models**: Import the optimized 3D models (GLB format) into Meta Spark Studio.
2. **Add Audio Files**: Import and add the dinosaur roar audio files.
3. **Use Patch Editor**:
   - Set up patches to control the interaction logic for the picker and info buttons.
4. **Testing and Optimization**: Continuously test and optimize the filter to ensure smooth performance.

## Contributing

Contributions are welcome! Please follow these steps to contribute:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/your-feature`).
3. Commit your changes (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature/your-feature`).
5. Open a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
