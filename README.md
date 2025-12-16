import random

print("🎮 Welcome to the Addition Game!")
print("Solve the addition problems below.\n")

score = 0

for i in range(5):  # number of questions
    num1 = random.randint(1, 10)
    num2 = random.randint(1, 10)

    print(f"Question {i + 1}: What is {num1} + {num2}?")
    answer = int(input("Your answer: "))

    if answer == num1 + num2:
        print("✅ Correct!\n")
        score += 1
    else:
        print(f"❌ Wrong! The correct answer is {num1 + num2}\n")

print(f"🏁 Game Over! Your final score is {score}/5")
 
