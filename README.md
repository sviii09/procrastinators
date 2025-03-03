# **Secure Data Hiding in Images Using Steganography**  

## **Overview**  
This project implements **image steganography** using Python and OpenCV, enabling secure and covert communication. It embeds **text messages** within images using the **Least Significant Bit (LSB) technique**, making modifications imperceptible to the human eye.  

## **Features**  
✔️ **Text Hiding & Extraction** – Embed and retrieve messages seamlessly.  
✔️ **Optimized LSB Algorithm** – Uses multiple channels for improved capacity.  
✔️ **Delimiter-Based Identification** – Ensures accurate extraction.  
✔️ **Custom Message Handling** – Supports user-defined secret messages.  
✔️ **Performance & Visualization** – Displays image differences for analysis.  

## **Technology Used**  
- **Python**  
- **OpenCV** – Image processing  
- **NumPy** – Array operations  
- **Google Colab** – Cloud-based execution  
- **Matplotlib** – Data visualization  

## **How It Works**  
🔹 **Encoding:** Converts text to binary and embeds it in the LSBs of image pixels.  
🔹 **Decoding:** Extracts the binary data and reconstructs the original message.  
🔹 **Optimization:** Uses multiple color channels for better efficiency.  

## **Installation**  
Run the following command to install dependencies:  
```bash
pip install opencv-python numpy
```

## **Usage**  
1️⃣ **Upload an Image**  
2️⃣ **Hide a Secret Message**  
```python
steg = Steganography()
steg.hide_data_optimized("input.jpg", "Secret Message", "output.png")
```
3️⃣ **Extract the Hidden Message**  
```python
hidden_text = steg.extract_data_optimized("output.png")
print("Extracted Text:", hidden_text)
```
4️⃣ **Visualize the Differences**  
- Displays original and modified images  
- Highlights modified pixels to show where data is hidden  

## **Results**  
✅ **Before & After Images** – Hidden data remains undetectable.  
✅ **Difference Analysis** – Shows where changes occur.  
✅ **Successful Message Retrieval** – Extracted text matches the original.  

## **Future Scope**  
🚀 **Adaptive Bit Selection** – Dynamically adjust bit manipulation.  
🔐 **Encryption Layer** – Enhance security by encrypting messages before embedding.  
🤖 **AI-Based Optimization** – Improve data-hiding efficiency.  

## **Contributors**  
👤 **Manasvi Vongur** – Developer  


## **GitHub Repository**  
[🔗 Steganography in Images](https://github.com/sviii09/procrastinators/blob/main/Steganography_in_Images.ipynb)


