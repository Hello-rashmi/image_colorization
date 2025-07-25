# Image Colorization with PyTorch
This project showcases an image colorization model developed using PyTorch. The goal is to take a grayscale image and intelligently predict its original colors. We've built a convolutional neural network (CNN) for this task, complete with features for visualizing the model's output and even exaggerating the predicted colors for a more vibrant look.

# How It Works
Think of it like an artist. My Encoder-Decoder neural network "looks" at the grayscale image (the "encoder" part, which understands the shapes and features). Then, it "paints" in the colors (the "decoder" part, which reconstructs the image with color).
I train it by showing it lots of real color pictures (from the CIFAR-10 dataset), converting them to grayscale, and asking the model to re-colorize them. It learns by trying to make its colorful guesses match the original pictures.

Get the code: git clone <your-repo-url> (replace with your repo!)

Set up: cd <your-repo-name> then python -m venv venv and source venv/bin/activate (or .\venv\Scripts\activate on Windows).

Install: pip install torch torchvision matplotlib numpy pillow

Run: Save the code as colorize.py and hit python colorize.py. Works great in Google Colab too!



# output
ter training (it runs for 30 "learning sessions" or epochs), the script will show you some cool comparisons:

Original: The actual colorful picture.

Grayscale: What the model sees.

Colorized: What the model creates!

I even added a fun feature to "exaggerate" the colors in the output, making them pop even more!




