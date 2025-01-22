**This is a deprecated repo. Please check out https://github.com/pirate2580/BugShot **

**How To Use:**
1. git clone <repo-ssh>
2. pip install -r requirements.txt
3. python main.py

**Make sure that you have the Arduino board connected via the COM6 port on a Windows system, if on a Mac or Linux, manually change the port to whatever desired.**

**Inspiration**
As "Patriotic" students dealing with "pest" issues in our apartments, we wanted a safe, effective way to keep insects away from specific areas without relying on harmful chemicals. Traditional repellents use poisons that can endanger pets, the environment, and even our health.

Our solution takes a new perspective by using AI-powered object detection to precisely target pests and repel them with water, avoiding the need for toxic substances. This eco-friendly not-a-guided-weapons-platform keeps insects out of key spaces like kitchens and desks while being safe for homes and the environment.

**What it does** 

Our project is a smart, eco-friendly "pest control system" that uses cutting-edge AI technology to keep specific areas "insect"-free. Here's how it works:

Intelligent "Insect" Detection: A fine-tuned YOLOv8 model identifies insects in real time, distinguishing between beneficial and harmful bugs, ensuring targeted action only against pests. Watergun Mechanism: Integrated with Arduino and motors, the system activates a watergun to repel harmful insects from designated areas with precision. This innovative approach combines AI and automation to create a safe, chemical-free solution for keeping spaces pest-free while protecting beneficial insects and the environment.

How we built it Our project combines hardware, AI, and backend software to create an innovative pest control system. Here's how we brought it to life:

CAD Modeling: We designed the gears and movement mechanisms in CAD, ensuring precise control of the watergun's aiming and shooting. Arduino Integration: We wrote Arduino code to control the servos and motors, enabling smooth and accurate movement of the watergun turret. Data Collection & Labeling: We painstakingly hand-labeled 5,000 images from online insect datasets to create a high-quality dataset for insect detection. Model Training: Using our labeled data, we fine-tuned YOLOv8 to accurately identify insects and classify them as harmful or beneficial. Hardware-Software Integration: The Python backend communicates with the Arduino, ensuring seamless coordination between the AI detection and the physical watergun mechanism through serial UART. This combination of mechanical design, AI-powered detection, and integrated hardware makes our system highly efficient and adaptable for targeted pest control.

**Challenges we ran into 😈 **

Our project presented numerous challenges that tested our technical and problem-solving skills:

Labeling 5,000 Images: Preparing the dataset was an exhaustive process, taking seven straight hours of manual labeling to ensure the quality and accuracy of the training data. Fine-Tuning the Model: Adjusting YOLOv8 to detect insects with precision required careful parameter tuning and experimentation, taking an additional iteration and three hours of focused effort. Hardware Integration: Setting up communication between the Python backend and the Arduino using PySerial proved tricky, requiring debugging to ensure smooth and reliable data exchange. 3D Printing CAD Designs: Printing our custom CAD-modeled gears and movement components posed challenges with calibration and print quality, requiring multiple iterations to achieve the desired functionality. We had to be resourceful. We walked for hours to the nearest 3D printer-equipped toronto public library. We had to take numerous detours and runs to the dollar store for superglue, hot glue, box cutters, and other miscellaneous items we needed on the fly that we did not have. Despite these hurdles, each challenge offered valuable learning opportunities and contributed to the success of our innovative pest control system.

**Accomplishments that we're proud of** 

High-Accuracy Model Training: We achieved an impressive 99% mAP and 80% mAP50-95 on our fine-tuned YOLOv8 model, ensuring reliable and precise insect detection. Seamless Hardware-Software Integration: Successfully bridging the gap between AI-powered detection and the physical watergun mechanism with high precision was a major technical milestone, showcasing our ability to integrate diverse systems. Creativity and Fun: This project combined technical innovation with a fun and creative approach to pest control, turning a challenging task into an enjoyable and rewarding experience. We’re proud of how we brought our idea to life, blending technology and creativity into a practical, eco-friendly solution.

**What we learned **

This project was a journey of firsts, and we gained valuable skills and insights along the way:

Fine-Tuning a Vision Model: We learned how to fine-tune an object detection model (YOLOv8) for the first time, understanding the intricacies of training and optimizing for high accuracy. Data Collection and Labeling: It was our first experience gathering and labeling an entire dataset from scratch, teaching us the importance of quality data for model performance. Software-Hardware Integration: We explored the challenges and nuances of connecting AI-powered software with physical hardware, learning how to bridge the two seamlessly. These experiences expanded our technical expertise and provided us with skills we’ll carry into future projects. Built With Python, Ultralytics, Pytorch, Arduino, UART
