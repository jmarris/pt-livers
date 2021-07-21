# Perceptual training with liver images
This repository contains the data and analysis for the paper and poster "How effective is perceptual training? Evaluating two perceptual training methods on a difficult visual categorisation task", presented at CogSci 2021. 

The `pt-analysis` markdown file contains the code to generate the analyses and figures presented in the paper and poster. 

## Data
`trainData` contains the data from the perceptual training experiment with medically naive participants. 
**Columns**
1. "participantID": unique participant identifier
2. "expCondition": the training condition (comparison or single-case)
3. "session": the training session number (1, 2, 3, or 4)
4. "trial_index": index for all entire experiment (e.g., icludes instructions, demographics, functions etc.)
5. "trial_type": identifes the trial action (e.g., pre-test, post-test, attention_check, grade, compare, feedback)
6. "key_answer": the correct grade 
7. "key_press": the participant's response
8. "correct": whether the response was correct
9. "diff": the absolute distance (error) between the correct reponse and the participant's response
10. "stimulus_L": the image that appeared on the left
11. "stimulus_R": the image that appeared on the right
12. "text_answer": the text description of the correct answer
13. "case_number": index for case number for each phase of the experiment (resets at each phase)
14. "trial_number": index for experiment trials (only the pretest, training, and post-test trials)
15. button_pressed: the button the participant pressed
16. "level": the difficulty level of the comparison (higher = more difficult) in the comparison condition
17. "age": the participant's age
18. "gender": the participant's gender
19. "country": the country where the participant resides
20. "time_elapsed": the time elapsed (ms  )up to that point in the experiment
21. "rt": response time for trial

`expertData` contains the ratings provided by the five radiology experts.
**Columns**
1. "participant": unique identifier for each expert
2. "graded": the grade that the expert gave an image (1-7)
3. "image": the image
