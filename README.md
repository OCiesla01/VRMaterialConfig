# VR Material Configurator

**_A Virtual Reality experience for testing, customizing, and visualizing PBR materials in real-time._**

## 🧠 About the Project

The VR Material Configurator is a Virtual Reality application built in Unreal Engine 5, designed to streamline and accelerate the material testing process. It allows users to select, modify, and visualize PBR materials in real-time across multiple environments and 3D models, providing a highly immersive and intuitive way to preview surface behavior under various lighting conditions.

This project focuses on enhancing productivity and creative control in the material creation and visualization workflow, offering a real-time, interactive testing environment for artists, designers, and technical developers.

## 🎥 Visual Overview

***here will be link to the video***

## 🕹️ User Instructions

### Installation
1. Download the zip file of the project
2. Unzip it on your PC
3. Launch **project.exe**
4. Make sure your VR headset is connected to your PC

### Using the Application
1. Rotate your left hand and look at it to open the material selection menu - here you can choose category and select material to apply to model.
2. Grab model to move it and rotate it.
3. Grab flashlight and press **interaction** button to turn light on/off. Use right joystick on the controller to control light intensity (left-right) and light cone size (up-down).
4. Press the big button to open **material properties control panel** - here you can dynamically adjust properties like: tiling, offset, brightness and many others. You can also change model's mesh here.
5. To save the material link, press the **Save Material** button. It will save link to the material in .txt file in project's **saved** folder.
6. To reset model position, press the **Reset Model** button.
7. Press **Menu Button** to open menu. From here you can reset your view, open level selection menu or quit the application.
8. After opening the **Level Selection Menu** you will be able to choose level you want to load.

## 🧑‍💻 Developer Instructions

### Engine
* **Version**: 5.6.1
* Uses only Blueprints with plugin support - FILE I/O, Enhanced Input, OpenXR

### Adding new Materials
_It is highly recommended to use appropriate folder in **Content > Materials > Usable** when adding new material_
1. Create new subfolder in appropriate material category folder - e.g. **Wood5** in **Wood**
2. In created subfolder, create new folder **Textures** where textures will be stored

_Recommended material folder structure example:_
<img width="1920" height="1080" alt="folder_structure" src="https://github.com/user-attachments/assets/6888d148-9b7b-4b2e-a657-0f814ccef354" />

3. Import textures to created **Textures** folder
4. Go to **Content > MasterMaterialTemplate** and create material instance from **M_Master**
5. Move created material instance to created subfolder (material subfolder, not **Textures** folder inside)
6. Add imported textures to material instance and save it
7. Open materials datatable under **Content > Data > DT_Materials**
8. Add new row and fill it with material data:
- **Category*** - choose fitting material category
- **Base Texture** - drag & drop base texture of the material
- **Material** - drag & drop created material instance
- **Name** - enter display name for the material
- **Link** - enter link to website from which textures were downloaded
9. Your material is ready to use in real-time

## 🧩 Contributions
If you'd like to improve the project:
* 🐞 Bug Reports
* ⚙️ Code or Blueprint Fixes
* 💡 Feature Suggestions
Feel free to write to me on my email **oskar.ciesla.development@gmail.com**
