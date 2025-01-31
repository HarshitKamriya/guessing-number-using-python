# guessing-number-using-python
import random
import time

print("🎲 Welcome to the Number Guessing Trick Game! 🎲")
while True:
    input("\nThink of a number between 1 and 100 and type 'yes' to continue: ")
    time.sleep(1)

    print("Now, add the same number again to your numberas your friend number ")
    time.sleep(1)

    friend_number = random.randint(1, 100)
    input("Enter 'yes' once you've added your friend's number: ")
    time.sleep(1)

    print(f"Now, add my number to your total: {friend_number}")
    time.sleep(1)
    
    input("Press 'yes' once you've added my number: ")
    time.sleep(1)

    print("Now, divide your total by 2.")
    time.sleep(1)

    input("Press 'yes' once you've divided the number: ")
    time.sleep(1)

    print("Now, subtract the friend's number that you added in the beginning.")
    time.sleep(2)

    print(f"🎉 The answer you got is: {friend_number // 2} 🎉")
    
    play_again = input("\nWant to play again? Type 'yes' to continue or 'no' to quit: ").strip().lower()
    
    if play_again == 'no':
        print("Thank you for playing! 😊")
        break
    else:
        print("\n🔁 Let's play again!")
