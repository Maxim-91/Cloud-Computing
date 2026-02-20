# Module 1 - a basic ML model using Google Teachable Machine
The model was created using Google Teachable Machine, an AutoML tool that simplifies the ML process by automating manual steps. It is trained to recognize six specific classes: Glass, Cup, Table, Chair, Sofa, and Candle.

### Project Structure: `my_model`
[cite_start]The `my_model` folder contains the exported **TensorFlow.js** files necessary for the application to function[cite: 170, 173]:
* [cite_start]`model.json`: The model architecture[cite: 170].
* [cite_start]`weights.bin`: The learned parameters (weights)[cite: 170].
* [cite_start]`metadata.json`: Information about the 6 object classes (Glass, Cup, Table, Chair, Sofa, and Candle)[cite: 158, 170].

### How to Use

1.  [cite_start]**Placement**: Ensure the `index.html` file and the `my_model` folder (containing the three files above) are in the same directory[cite: 173].
2.  [cite_start]**Run a Server**: To function correctly, the application must be opened via a web server[cite: 174]. 
    * [cite_start]**Recommended**: In Visual Studio Code, right-click `index.html` and select **"Open with Live Server"**[cite: 175].
3.  **Interaction**: 
    * [cite_start]Click the **"Launch Camera"** button[cite: 181].
    * [cite_start]The model will scan the video frame for objects[cite: 171].
    * [cite_start]When an item is detected (e.g., a **Chair** or **Candle**), its name will highlight in **green** on the UI list[cite: 172, 184].

---
