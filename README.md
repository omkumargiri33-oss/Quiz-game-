# Quiz-game-
questions = {
    "Q(1):- len([1, [2, 3], 4]) ka output kya hoga\na.2\nb.3\nc.4\nd.error": "b",
    "Q(2):- Python me list ko sort karne ke liye kaunsa method use hota hai?\na.sort\nb.order\nc.arrange\nd.sorted": "a",
    "Q(3):- Who is the father of computer?\na.hitler\nb.charles babbage\nc.mr ford\nd.robort wald": "b",
    "Q(4):- which keyword used for define function?\na.func\nb.def\nc.function\nd.define": "b"
}

score = 0

print("Welcome to Quiz Game!")
print("----------------------")

for question, answer in questions.items():
    user_answer = input(question + " : ").lower().strip()
    
    if user_answer == answer:
        print("Correct!\n")
        score += 1
    else:
        print(f"Wrong! Correct answer is: {answer}\n")

print("----------------------")
print(f"Your Final Score is: {score}/{len(questions)}  ({score/len(questions)*100:.1f}%)")
