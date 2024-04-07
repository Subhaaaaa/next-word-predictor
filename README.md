# next-word-predictor

- What is a next word predictor 

    We will pretend it as a text generator under supervised learning(classification) which will have the sentence as a input and the next predicted word as output.

    Ex . I am from maharastra and I speak marathi.

![image](https://github.com/Subhaaaaa/next-word-predictor/assets/101266414/afa70de9-f730-4c61-a258-278266feaec6)

  

    But since the model doesnot undertsand english words we will use integer encoding to convert them into vector .
    Ex input = [2 3 4] output = [5]
 
- Architecture of the model 
        
        1st layer - Embedding to reduce the dimensions of the sarse vectors created due to padding and make it dense and capture semantic relationships(Converts each word into a 100 dim dense vector for input , so for 283 words = 28300 dense vectors)

        2nd layer - LSTM - To train and predict the next word 

        3rd layer - Dense with activationfunction as softmax to predict the outputs from different multiclasses through conditional probabilities

