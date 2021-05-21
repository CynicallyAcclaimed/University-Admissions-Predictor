# University Admissions Predictor
Building a model that can predict admissions to universities, based on previous years' admissions statistics.

As part of my application designed for students applying for graduate studies at HCI programmes (work in progress), I'm building a simple predictor that would predict a student's chances of admission at a particular university.
This is based on statistics obtained from students who had applied in the previous years. I collected this data through Yocket, GradCafe, and a certain crowdsourced Google datasheet. 

As Human-Computer Interaction is still a growing field, there isn't a lot of data about it out there. I managed to obtain about 250 records, split across different universities. While the application is meant to generate more data over time, allowing for the model to learn iteratively, it wasn't enough for the present. 
So, to improve the model, I looked into synthetically generating more data based on the existing collection. 

I had already explored the different types of GAN models and for my purpose, CTGAN was the best way forward. Accuracies with different models and number of data points were compared, and an average accuracy of 75% for each university was achieved. 


### Datasheet Info:
GRE and TOEFL scores can be NA because:
(a) University doesn't require the scores;
(b) The student has a waiver or doesn't need to submit the scores

CGPA converted to 4.0 scale for uniformity

Student Status based on GradCafe's notation: 
I for International Students;
A for Domestic Students;
U for International Students with a domestic undergraduate degree

QS and THE rankings are from 2020 and are liable to change
