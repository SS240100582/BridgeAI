# BridgeAI Demo - How it works

def clean_question(question):
    # Step 1: Remove private words
    private_words = ["Lahore", "my name", "diabetes", "for me"]
    clean = question
    for word in private_words:
        clean = clean.replace(word, "")
    # Step 2: Make it general
    clean = clean.replace("best medicine", "Best medicine for diabetes in Pakistan?")
    return clean

# User asks Apple
user_question = "I have diabetes, best medicine for me in Lahore?"

print("User asks Apple:")
print(user_question)
print("")

# Apple cleans it
safe_question = clean_question(user_question)

print("Apple sends to Meta (safe version):")
print(safe_question)
print("")

print("Meta answers, Apple shows answer to user privately.")
print("Meta never knows who asked it.")
