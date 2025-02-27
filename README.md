# Edge Detection Backend

## 📋 Overview
Edge Detection Backend is a C# application that implements edge detection algorithms like **Sobel** and **Prewitt**. The project allows users to apply these operators to input images, producing output images highlighting edges for further analysis. It includes a testing suite to ensure robustness and correctness.

## 🎯 Features
- **Edge Detection Algorithms**:
  - Sobel Operator
  - Prewitt Operator
- **Interactive User Interface**:
  - Select input images and output paths using file dialogs.
- **Unit Testing**:
  - Verifies operator selection logic, output dimensions, and algorithm correctness.

## 📁 Project Structure
```
EdgeDetectionBackend/               # Main application code
   ├── Program.cs                   # Entry point
   └── EdgeDetection
       ├── Prewitt.cs               # Prewitt operator implementation
       └── Sobel.cs                 # Sobel operator implementation
   └── EdgeDetectionUML
       ├── EdgeDetectionUML.puml    # UML Source Code
       └── out/testuml # UML
   ├── README.md                    # Documentation
   ├── ...
   └── EdgeDetectionBackend.Tests/  # Unit tests
       ├── EdgeDetectionTests.cs
       └── ...
```

## 🚀 Getting Started

### Prerequisites
Ensure you have the following installed:
- .NET SDK 9.0+ (supports `net9.0-windows`)
- Visual Studio or any IDE supporting C#
- dotnet add package NUnit
- dotnet add package NUnit3TestAdapter
- dotnet add package System.Drawing.Common
- dotnet add package System.Windows.Forms

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/Mikehuntisbald/EdgeDetectionBackend.git
   cd Aug_test
   ```
2. Build the project:
   ```bash
   dotnet build
   ```
3. Run the application:
   ```bash
   dotnet run
   ```

### Running Tests
To verify functionality:
```bash
cd EdgeDetectionBackend.Tests
dotnet test
```

## 🖼️ How to Use
1. Launch the application.
2. Select an input image via the file dialog.  
   ![Select Input Image](https://github.com/Mikehuntisbald/Aug_test/blob/main/Example/pic_selec.png)
3. Choose an output file path for the processed image.  
   ![Specify Output File Path](https://github.com/Mikehuntisbald/Aug_test/blob/main/Example/output_name.png)
4. Select the edge detection operator:
   - `1` for Sobel
   - `2` for Prewitt  
   ![Select Edge Detection Operator](https://github.com/Mikehuntisbald/Aug_test/blob/main/Example/operator_selec.png)
5. View the processed image saved at the specified output location.

## 🧪 Testing Details
The following aspects are covered by the unit tests:
- Operator selection logic
- Correct handling of input and output image dimensions
- Validation of pixel intensity correctness

## 📖 Example
**Input Image**:
![Input Image](https://github.com/Mikehuntisbald/Aug_test/blob/main/Example/2d-atk.png)

**Output Image (Sobel)**:
![Output Image Sobel](https://github.com/Mikehuntisbald/Aug_test/blob/main/Example/example.jpg)

## 📜 License
This project is licensed under the [MIT License](LICENSE).

## 📞 Contact
If you have any questions or feedback, feel free to reach out:
- **Author**: Haoyi Wang
- **GitHub**: [Mikehuntisbald](https://github.com/Mikehuntisbald)
- **Email**: db72702@gmail.com
