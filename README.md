print("Mind Exercise Quiz Made by Priyansh Saxena")
questions = ("How many elements are in the periodic table?: ",
            "Which animal lays the largest eggs?: ",
            "What is the most abundant gas in Earth's atmosphere?: ",
            "How many bones are in the human body?: ",
            "Which planet in the solar system is the hottest?: ",
            "An integer can be:",
            "A rational number can be represented in the form of:",
            "The value of ½ x  3/5 is equal to:",
            "The value of (½) ÷ (3/5) is equal to:",
            "The value of ½ + ¼ is equal to:")

options = (
    ("A 116","B 117","C 118","D 119"),
    ("A Whale","B Crocodile","C Elephant","D Ostrich"),
    ("A Nitrogen","B Oxygen","C Carbon-dioxide","D Hydrogen"),
    ("A 206","B 207","C 208","D 209"),
    ("A Mercury","B Venus","C Earth","D Mars"),
    ("A Only Positive","B Only Negative ","C Both Positive & Negative","D None of these"),
    ("A P/Q ","B PQ ","C P+Q","D P-Q"),
    ("A 1/2","B 3/10","C 3/5 ","D 2/5"),
    ("A 3/10","B 2/6","C 3/4","D 5/6"),
    ("A 3/4","B 3/2","C 2/3","D 1"),)
    
answers = ("C","D","A","A","B","C","A","B","D","A")

guesses = []
score = 0
question_num = 0

for question in questions:
    print("_ _ _ _ _ _ _ _ _ _")
    print(question)
    print("Options:")
    for option in options[question_num]:
        print(option)
    response = input("Enter your answer:")
    guesses.append(response.upper())
    if guesses[question_num] == answers[question_num]:
        score += 1
        print("Correct!")
    else:
        print("Incorrect!")
    print("Your current score is:", score)
    question_num += 1

print("Game over! Your final score is:", score)



