# Electrochemistry Analysis

Part of the paper done by Dr Linda Sellou and Chia Kwang Yang.
The data is anonymized but each number is present in both pre-course and post-course data. Those that are not present in either are removed early.

There are three parts to the code itself.

## Part 1 - students’ attitudes towards electrochemistry
Part 1 consists of 15 questions, with the different questions trying to find out different things:

1. Attitudes towards Electrochemistry lessons
2. Attitudes towards Electrochemistry labs
3. Beliefs towards Electrochemistry
4. Tendencies to learn about Electrochemistry
5. Anxieties towards Electrochemistry 

These are all on a likert scale and are compared pre-course and post-course. We map the responses to a scale of -2 to 2 (integer-wise) then calculate the Cronbach's alpha for both pre-course and post and compare the two alphas to see if the alphas have increased/decreased.

## Part 2 - students’ misconceptions regarding electrochemistry
Part 2 consists of 10 questions, with the different questions trying to find out if students’ misconceptions regarding electrochemistry have been cleared and their confidence level regarding these misconceptions. 

The statements provided in the survey are all False. We map the responses as such: 
`map_d = {'True, I am confident': (0,1),
 'False but I am not sure': (1,0),
 'True but I am not sure': (0,0),
 'I have no idea': (0,0),
 'False, I am confident': (1,1)}`
After that, we calculate the differences in terms of correctness and confidence level and we visualised it. Lastly, we used a one-tailed t-test to see if the change in the correctness and confidence level is statistically significant, which they both are. 

## Part 3 - rating on how useful, interesting, and easy to understand and perform the experiments were.
Part 3 was exclusive to the post-course survey and it was to rate how useful, interesting and easy to understand and perform the experiments were. We visualised the responses.