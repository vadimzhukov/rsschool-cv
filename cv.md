# Vadim Zhukov
![picture of me](/rsschool-cv/Avatar.png "picture of me")

## My contacts (*not real*)
- email: **vadim@gmail.com**
- mobile: **+7 999-999-99-99**
- discord: **Vadim Zhukov(@vadimzhukov)**
- github: **@vadimzhukov**
- reside in: **Moscow**
- relocation readiness: **Europe**
****
## About me
I am accomplished and energetic Senior Project Manager with a solid history of achievement over 16+ years in Software development. Nowadays interested in frontend development.

## Skills
- HTML5
- CSS, SCSS, SASS
- JS core

- IT-project management
- Analysis
- Management consulting
****
## Projects

### Code sample

Here is the sample of code of my game pet-project:
```
fetch('https://opentdb.com/api.php?amount=10&category=9&difficulty=easy&type=multiple')
    .then(res => {
        return res.json();
    })
    .then(loadedData => {

        questions = loadedData.results.map(loadedQuestion => {
            
            //Start formatting the required structure of question+choices objects
            
            let adoptedQuestion = {
                question: htmlDecode(loadedQuestion.question)
            }

            const answerNumber = (Math.floor(Math.random() * 3) + 1);

            adoptedQuestion.answer = answerNumber;
            //temp array to save answers for current question
            const answers = [...loadedQuestion.incorrect_answers.map(answer => htmlDecode(answer))];
            answers.splice((answerNumber - 1), 0, htmlDecode(loadedQuestion.correct_answer));

            answers.forEach((item, index) => {
                adoptedQuestion['choice' + (index + 1)] = item;
            });
            return adoptedQuestion;
        });
        startGame();
    }).catch(err => console.error("===ERROR===" + err));
});
```

### Working project

You can see [this project at my GitHub](https://github.com/vadimzhukov/Let-s-quizzz "GitHub link") and play the [game](https://vadimzhukov.github.io/Let-s-quizzz/ "my quiz game") with your friends!

****
## Experience & education
### FrontEnd experience

I'm learning web-development for 2 months, but my overla it experience in different positions if more than 16 years.


### Education and cources

- IT masters degree.
- Сompleted JS learning course at learn.javascript.ru

****
## Languages

- Russian - **native**
- English - **upper intermediate (B1)**