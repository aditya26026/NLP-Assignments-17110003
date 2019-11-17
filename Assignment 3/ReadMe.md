The data was preprocessed to remove punctuation marks, emojis all ‘RTs’ and link to other usernames(@). I have even removed all hyperlinks from the text. I have also removed various stop words from the text.

I have used two models, one being sub word LSTM and the other being char CNN.

The first model was proposed by Prof. Aditya Joshi from IIIT Hyderabad and says that sub word level embeddings can be generated using 1D convolutions on character level inputs of a given sentence.
After the embeddings are generated we use LSTM which is utilised to remember past information and propagate it further to predict the sentiments conveyed by the sentence..
We use adamax optimizer to train this setup.

The accuracy from this model comes out to be 0.543606206718902.
The f1 score from this model comes out to be 0.5136723921476296.
The precision from this model comes out to be  0.5781007611923769
The recall from this model comes out to be  0.46388443036791216.

The other model used by me is char CNN. It has 3 convolution layers with back to back 2 max pooling layers. At the end it has a fully connected layer with adam being used as an optimizer to train this setup.
 
The accuracy from this model comes out to be 0.5013376137131098.
The f1 score from this model comes out to be 0.5010328342278033.
The precision from this model comes out to be 0.5023818146168325.
The recall from this model comes out to be 0.49973247727651277.
