Here's a simple **README** text based on what you've requested:

---

### **Handwritten Digit Recognition**

This project uses a Convolutional Neural Network (CNN) to predict handwritten digits (0-9) from images.

## How to Use:

   Example code:
   ```python
   image = cv2.imread('9.png')[:,:,0]   # Read the image (using 0th channel)
   image = np.invert(np.array([image]))  # Invert the image
   output = model.predict(image)         # Predict the digit
   plt.imshow(image[0])                  # Display the image
   print(np.argmax(output))              # Print the predicted digit
   ```

## Notes:
- Make sure to change the filename (`'9.png'`) in the script to the desired image file you want to test.
- You can change the image name by simply replacing `9.png` with any other image (e.g., `1.png`, `2.png`, etc.).
- The prediction will output the digit that the model has recognized.
