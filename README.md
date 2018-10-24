# Face Recognition for Augmented Reality

Example project to show how we can add face recognition functionality to an AR app, using the popular DLib C++ framework. We start by using Apple's built in `Vision` framework to compute bounding boxes around faces, then passed these bounding boxes (along with the current image) to our DLib function, which computes the 68 face landmarks, then passes these to the actual recognition network that generates an embedding. We then save these embeddings for each person, and use them to recognise who we might be looking at. Finally, we show a floating (and potentially meaningless!) label at the 3D, real-world, position of the person.
