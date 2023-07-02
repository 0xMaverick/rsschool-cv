# Ilya Nos
***
## Contact information
* **Location:** Minsk, Belarus
* **Phone number:** + 375 29 3890699
* **E-mail:** 3890699@gmail.com
* **Github:** [0xMaverick](https://github.com/0xMaverick)

***
## About me
I am 33 years old and I am fond of programming and development. Despite the fact that I studied at a specialized university I began to work in a completely different field. Now I'm interested in development again and I want to grow in this direction. I consider diligence and perseverance to be my strengths. In addition I alwats strive to acquire new knowledge and skills.
***
## Skills
* HTML/CSS
* Java Core
* SQL
* JavaScript basics

***
## Code example
Write a program that enters a string of text from the keyboard.
The program should display two lines:
1. The first line contains only vowels from the input line.
2. the second - only consonants and punctuation marks from the entered string.
   
Connect the letters with a space, each line must end with a space.
```
public class Solution {
    public static char[] vowels = new char[]{'а', 'я', 'у', 'ю', 'и', 'ы', 'э', 'е', 'о', 'ё'};

    public static void main(String[] args) throws Exception {
        BufferedReader reader = new BufferedReader(new InputStreamReader(System.in));
        char[] charArray = reader.readLine().toCharArray();
        List<Character> vowelsList = new ArrayList<Character>();
        List<Character> consonantsList = new ArrayList<Character>();
        for (char ch : charArray) {
            if (ch != ' ') {
                if (isVowel(ch)) {
                    vowelsList.add(ch);
                } else {
                    consonantsList.add(ch);
                }
            }
        }
        for (char ch : vowelsList) {
            System.out.print(ch + " ");
        }
        System.out.println("");
        for (char ch : consonantsList) {
            System.out.print(ch + " ");
        }
    }

    // метод проверяет, гласная ли буква
    public static boolean isVowel(char character) {
        character = Character.toLowerCase(character);  // приводим символ в нижний регистр - от заглавных к строчным буквам
        for (char vowel : vowels) {  // ищем среди массива гласных
            if (character == vowel) {
                return true;
            }
        }
        return false;
    }
}
```
***
## Experience
https://github.com/0xMaverick/rsschool-cv

***
## Education
* BSUIR - information systems and technologies (economics)
* studied Java at https://javarush.com

***

## English level
B2 (according to [EPAM English test](https://examinator.epam.com/Main/PersonalAssignments))

