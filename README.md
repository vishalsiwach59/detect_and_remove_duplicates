# detect_and_remove_duplicates
detect and remove duplicate images from a dataset for deep learning.

The dataset I was using was crafted by combining images from multiple sources. 
I knew there were going to be duplicate images in the dataset — I therefore needed a method to detect and remove these duplicate images from my dataset.

Having duplicate images in your dataset creates a problem for two reasons:

          1. It introduces bias into your dataset, giving your deep neural network additional opportunities to learn patterns specific to the duplicates.
          2. It hurts the ability of your model to generalize to new images outside of what it was trained on.
          
While we often assume that data points in a dataset are independent and identically distributed, that’s rarely (if ever) the case when working with a real-world dataset. 
When training a Convolutional Neural Network, we typically want to remove those duplicate images before training the model.

Secondly, trying to manually detect duplicate images in a dataset is extremely time-consuming and error-prone .
it also doesn’t scale to large image datasets. We therefore need a method to automatically detect and remove duplicate images from our deep learning dataset.
          
