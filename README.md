# 🤖 CodeAlpha AI ChatBot (Java)

This is a simple **rule-based AI chatbot** built using **Java** as part of my internship with **CodeAlpha**. It simulates basic conversation using keyword matching logic and runs entirely in the console.

---

## 💡 Features

- Responds to common greetings and phrases
- Rule-based pattern matching
- Console-based interaction
- Beginner-friendly and easy to extend

---

## 📜 Code


```java
import java.util.Scanner;

public class AIChatBot {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        String input;

        System.out.println("🤖 AI ChatBot: Hello! I'm your assistant. Type 'bye' to exit.");

        while (true) {
            System.out.print("You: ");
            input = scanner.nextLine().toLowerCase();

            if (input.contains("hello") || input.contains("hi")) {
                System.out.println("AI: Hello there! How can I help you?");
            } else if (input.contains("how are you")) {
                System.out.println("AI: I'm just code, but I'm doing great!");
            } else if (input.contains("name")) {
                System.out.println("AI: I'm ChatBot, your virtual assistant.");
            } else if (input.contains("bye")) {
                System.out.println("AI: Goodbye! Have a nice day.");
                break;
            } else {
                System.out.println("AI: Sorry, I don't understand that.");
            }
        }

        scanner.close();
    }
}
🤖 AI ChatBot: Hello! I'm your assistant. Type 'bye' to exit.
You: hello
AI: Hello there! How can I help you?
You: what's your name?
AI: I'm ChatBot, your virtual assistant.
You: bye
AI: Goodbye! Have a nice day.
