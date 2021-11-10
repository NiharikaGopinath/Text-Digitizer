 I'll address the problem of handwritten scribes, which are typically given by doctors and nurses. I'll be converting handwritten scripts into digital records that can be stored in non-relational databases. The data for the model was taken from the IAM Handwriting database. This model is based on 657 distinct writers' handwriting. Multiple paragraphs were created by each writer, and sentences were extracted from those paragraphs.
# Model

To classify writers, I developed a multi layer CNN in Keras, followed by an RNN in Tensorflow. This project was inspired by a paper authored by Alex Graves, which is linked below. They were able to categorise and read English material with ease. 

# Results

Model's performance has been calculated based on a test set which has writings from among 50 writers. The model was not exposed to this data during training and validation Classification accuracy on Test Set : 94.1%

# References

IAM handwriting database http://www.fki.inf.unibe.ch/databases/iam-handwriting-database/download-the-iam-handwriting-database
Alex Graves work on RNN https://arxiv.org/pdf/1308.0850.pdf
