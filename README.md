# Temperature Application

🌟 **Description**
This project consists of two main components:

1. **TemperatureServer**: A SOAP web service that provides methods to convert temperatures between Fahrenheit and Celsius.
2. **TemperatureClient**: A Windows Forms application that allows users to input temperatures and perform conversions through a user-friendly interface.

## 🗂️ **Project Structure**

```
TemperatureWS/
├── TemperatureServer/
│   ├── WebService1.asmx       # Main web service
│   ├── WebService1.asmx.cs    # Code-behind for WebService1
├── TemperatureClient/
│   ├── Form1.cs               # Main form of the WinForm application
│   ├── Program.cs             # Application entry point
│   ├── App.config             # Application configuration file
```

## ⚙️ **System Requirements**

### **Software:**
- .NET Framework >= 4.7
- Visual Studio 2019 or newer

### **Hardware:**
- **Processor**: 1.6 GHz or higher
- **RAM**: Minimum 2GB
- **Free Disk Space**: Minimum 1GB

## 🚀 **Setup Instructions**

### Step 1: Clone the repository
```bash
git clone https://github.com/PhamTrung1204/temp.git
```

### Step 2: Run TemperatureServer
1. Configure the URL for the web service in `WebService1.asmx` if necessary.
2. Press `F5` in Visual Studio to run the service.

### Step 3: Run TemperatureClient
1. In Visual Studio, set the **TemperatureClient** project as the startup project.
2. Press `F5` to run the application.

## 🌐 **Web Service API**
The web service provides two main methods:

1. **Convert Fahrenheit to Celsius**
   - **Method**: `FahrenheitToCelsius`
   - **Parameter**: `fahrenheit (double)` - Input temperature in Fahrenheit
   - **Returns**: Equivalent temperature in Celsius (`double`)

2. **Convert Celsius to Fahrenheit**
   - **Method**: `CelsiusToFahrenheit`
   - **Parameter**: `celsius (double)` - Input temperature in Celsius
   - **Returns**: Equivalent temperature in Fahrenheit (`double`)

## 💡 **Usage Instructions**

### **Components:**

1. **TemperatureServer**
   - `WebService1.asmx`: The main web service that provides temperature conversion methods.
   - **Namespace**: `http://tempuri.org/`

2. **TemperatureClient**
   - **WinForm Interface:**
     - **Textbox**: Input temperature
     - **Label**: Display conversion results
     - **Button**: Perform conversions between Fahrenheit and Celsius

### **Steps to Use:**
1. Start **TemperatureServer** to launch the web service.
2. Open the **TemperatureClient** application to input a temperature and select a conversion.
3. View the result on the interface.

## 🔧 **Connecting Client to Server**
1. In Visual Studio, right-click on the **TemperatureClient** project.
2. Select **Add > Service Reference**.
3. In the **Add Service Reference** window, click **Advanced**.
4. Click **Add Web Reference**.
5. Enter the URL of `WebService1.asmx` (e.g., `http://localhost:port/WebService1.asmx`).
6. Click **Go** to load the service information.
7. Select the service and click **Add Reference**.

## 📋 **Testing**
- Use built-in tests in Visual Studio to validate each API method.
- Ensure correct results for test cases (e.g., `32°F = 0°C`).

## 🛠️ **Error Handling**
- The application validates input using `double.TryParse` to ensure correct formatting.
- Error messages are displayed for invalid inputs or connection issues with the web service.

## ✅ **Outcomes**
- **Completed Application**: Accurate temperature conversion between Fahrenheit and Celsius.
- **SOAP Web Service**: Successfully implemented and compatible with various platforms.
- **User Interface**: Intuitive and user-friendly with effective input validation and error handling.
- **Practical Knowledge**: Gained in-depth experience building .NET Framework-based applications.

## 📜 **License**
This project is licensed under the MIT License.

## 📧 **Contact Information**
- **Author**: PhamTrung1204
- **Email**: trungpham.31221024740@st.ueh.edu.vn
