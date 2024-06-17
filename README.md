### Enhancing E-commerce Search with Multimodal GANs

The goal of this project is to develop a GAN to enhance e-commerce search by synthesizing images from multimodal inputs (image + text).

**Implementation Details:**

- **Model Architecture:** The GAN architecture consists of a generator and discriminator. The generator uses BERT for text and CNN for images, combines features, and upscales via transpose CNN layers. The discriminator employs CNN layers, LeakyReLU activations, and a final Sigmoid layer.

- **Data Preprocessing:** The Fashion MNIST dataset is used for grayscale image generation. Images are scaled to the range [-1, 1] for consistency.

- **Training:** The model is trained with adversarial training using Adam optimizers and binary cross-entropy loss. The training process monitors losses and accuracies, and sample images are generated at intervals.

- **Evaluation:** The model is evaluated on its ability to generate realistic images, using metrics such as loss, accuracy, and visual inspection of generated samples.

- **Deployment:** The project is set up to run on Google Colab with TensorFlow and Matplotlib, with a local/server deployment option using a tkinter GUI for user interaction.

**Performance:**

- **Base Case:** The initial performance of the GAN is evaluated over 30,000 epochs with a batch size of 32, showing improved generation of fashion item images over time.

- **With Optimization Techniques:** Techniques such as hyperparameter tuning and GPU acceleration are applied to improve image quality and training efficiency.

- **Metrics:** The model's performance is evaluated using accuracy, loss, and visual quality of generated images.

**Code:**

You can find the code for the entire project in the `code` folder.

## Detailed Report

A comprehensive report detailing the model architecture, training process, evaluation metrics, and performance graphs is available in `report.pdf`.

For questions or feedback, please [email](mailto:gayatriwalke@gmail.com).
Thank You
