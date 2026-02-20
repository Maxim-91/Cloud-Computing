# Module 1 - a basic ML model using Google Teachable Machine
The model was created using Google Teachable Machine, an AutoML tool that simplifies the ML process by automating manual steps. It is trained to recognize six specific classes: Glass, Cup, Table, Chair, Sofa, and Candle.

### Project Structure: `my_model`
The `my_model` folder contains the exported **TensorFlow.js** files necessary for the application to function:
* `model.json`: The model architecture.
* `weights.bin`: The learned parameters (weights).
* `metadata.json`: Information about the 6 object classes (Glass, Cup, Table, Chair, Sofa, and Candle).

### How to Use

1.  **Placement**: Ensure the `index.html` file and the `my_model` folder (containing the three files above) are in the same directory.
2.  **Run a Server**: To function correctly, the application must be opened via a web server. 
    * **Recommended**: In Visual Studio Code, right-click `index.html` and select **"Open with Live Server"**.
3.  **Interaction**: 
    * Click the **"Launch Camera"** button.
    * The model will scan the video frame for objects.
    * When an item is detected (e.g., a **Chair** or **Candle**), its name will highlight in **green** on the UI list.

---
