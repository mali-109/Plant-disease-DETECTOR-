# Plant-disease-DETECTOR-
import numpy as np
from PIL import Image
import matplotlib.pyplot as plt

# Simulated prediction probabilities (mocking the model's output)
predictions = [[0.85, 0.15]]  # Mocked probabilities for "Healthy" and "Diseased"
class_labels = ["Healthy", "Diseased"]
predicted_class = np.argmax(predictions)
predicted_label = class_labels[predicted_class]

# Load the uploaded image
img_path = 'uploaded_image.jpg'  # Replace with your image file path
img = Image.open(img_path).resize((128, 128))  # Resizing for consistency

# Plot the image with prediction
plt.figure(figsize=(6, 6))
plt.imshow(img)
plt.title(f"Predicted Health Status: {predicted_label}\nConfidence: {predictions[0][predicted_class] * 100:.2f}%")
plt.axis('off')

# Save the output image
output_path = "predicted_health_status.png"  # File name for saving
plt.savefig(output_path)
plt.show()

print(f"Output saved as {output_path}")
FarmAid Robo Machine Concept and Purpose

Purpose of FarmAid Robo Machine: The FarmAid Robo Machine is envisioned as a smart agricultural assistant designed to address the challenges faced by farmers, including improving efficiency, minimizing losses, and ensuring sustainable farming practices. Its key objectives are:

1. Disease Detection and Prevention: Equipped with advanced sensors and AI algorithms, the machine can detect early signs of plant diseases, pests, or deficiencies. This enables timely intervention and prevents large-scale crop damage.


2. Precision Farming: It assists in tasks like targeted pesticide spraying, irrigation management, and nutrient application, reducing wastage and promoting sustainable use of resources.


3. Harvesting Assistance: The robot can assist in identifying and harvesting mature crops, optimizing labor usage and reducing human effort.


4. Data Collection and Analysis: Continuous monitoring of soil health, weather conditions, and crop growth to provide actionable insights for better decision-making.


5. Environmentally Friendly Farming: By optimizing the use of fertilizers, pesticides, and water, the machine supports eco-friendly and sustainable agricultural practices.



Key Features and Components:

1. High-Resolution Cameras and Sensors: To capture detailed images of plants and the environment.


2. Machine Learning Models: For disease detection, plant health assessment, and growth prediction.


3. Autonomous Navigation: Using GPS and LiDAR for precise movement across fields.


4. Modular Design: Customizable attachments for various tasks like sowing, weeding, and spraying.


5. Cloud Connectivity: For data storage, remote monitoring, and real-time decision-making.



The FarmAid Robo Machine serves as an advanced technological partner to farmers, aiming to increase yields, reduce costs, and promote sustainable farming practices.

