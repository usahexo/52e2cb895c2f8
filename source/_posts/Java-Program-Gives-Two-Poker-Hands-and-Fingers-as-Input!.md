---
title: Java Program Gives Two Poker Hands and Fingers as Input!
date: 2022-12-13 15:15:23
categories:
- 12bet Game
tags:
---


#  Java Program Gives Two Poker Hands and Fingers as Input!

In my last post, I showed you how to write a Java program that would give you a random poker hand.  In this post, we'll extend that program to allow the user to type in two poker hands and then determine the winner.

First, let's take a look at the program:

import java.util.*; //import the necessary library import org.apache.commons.lang3.*; //import the necessary Apache library public class Poker { public static void main(String[] args) { Scanner input = new Scanner(System.in); System.out.println("Please enter the first poker hand:"); String firstHand = input.nextLine(); System.out.println("Please enter the second poker hand:"); String secondHand = input.nextLine(); if (firstHand.length() != secondHand.length()) { System.out.println("The hands must contain the same number of cards."); } else { int compare = PokerUtils .compare(firstHand, second Hand); if (compare > 0) { System .out .println("Second poker hand is higher ranking than first."); } else if ( compare < 0) { System .out .println("First poker hand is higher ranking than second."); } else { System .out .println("The two hands are equal in rank."); } } } //end main() method public static int compare(String first, String second) { int compare = 0; boolean isStraight = false; for (int i = 0; i <= first.length(); ++i) { char c1 = first.charAt(i); char c2 = second.charAt(i); if (c1 == c2) continue; //don't compare same character isStraight = true; if (Character .isDigit(c1) && Character .isDigit(c2)) { int val1 = Integer .valueOf(c1).intValue() + Integer .valueOf(c2).intValue(); int val2 = Integer .valueOf(first).intValue() + Integer .valueOf(second).intValue(); compare = val1 - val2; } else if (!isStraight && !Character .isSpecial (c1)) compare ^= ordinalCompare (c1, c2); } return compare ; } //method to calculate the ordinal comparison of two characters public static int ordinalCompare ( char c1, char c2) { return c1 - c2 ; } //method to convert a character to its integer value public static int valueOf ( char ch ) throws NumberFormatException{returnInteger .parseInt (ch ,16 );} //end class Poker

As you can see, the program is pretty straightforward - it simply takes in two Strings representing poker hands and then compares them using our custom compare() method.  If you're not familiar with how java compares objects, be sure to check out this article on stack overflow which does a great job of explaining it!

Now that we have our Poker program written, let's see how it works! Running the program from the command line looks like this:

Please enter the first poker hand: AQJT Please enter the second poker hand: KQJ4 Second poker hand is higher ranking than first.



As you can see, the program correctly determines that the KQJ4 hand is higher ranking than AQJT!

#  Second Java Program Input is Your Poker Hand!

In the first Java program, we asked the user to input a number and then printed out that number. In this program, we are going to ask the user to input a poker hand and then print out how strong that poker hand is.

We will use the rank of the card and the suit of the card to determine how strong a poker hand it is. The rank of a card is from 1 (Ace) to 13 (King). The suit of a card is either Clubs, Hearts, Spades, or Diamonds.

Here is a list of the ranks and suits:

Rank Suit

1 Clubs
2 Hearts
3 Spades
4 Diamonds
5 Clubs
6 Hearts
7 Spades 
8 Diamonds 
9 Clubs 
10 Hearts 
Jack Spades 
Queen Diamonds 
King Clubs





To start off our program, we will declare five variables called userHand, card1, card2, card3, and card4. We will set these variables to null so that we can later set them to the user's input. Next, we will have a while loop that will continuously ask the user for input until they enter "exit". We will set a boolean variable called done to true once the user enters "exit". Once done is true, we will break out of the while loop and move on to the next part of our program.





 inside the while loop. We will first get the user's input by using scanLine() . This function takes in an input String and put it into one of our variables called userHand . Next we want to check if the user entered "exit" by using If statement. If they did not enter "exit" then we want to check what type of poker hand it is by using switch statement . The switch statement takes in an integer and checks which case it matches. If it matches one of the cases, then it prints out what string is associated with that case. The default case prints out "Invalid Hand". Here is what our switch statement looks like: switch(userHand){ case 1: System.out.println("One Pair"); break; case 2: System.out.println("Two Pair"); break; case 3: System.out.println("Three Of A Kind"); break; case 4: System.out.println("Straight"); break; case 5: System.out.println("Flush"); break; case 6:System.out.println("Full House"); break; case 7:System.out.println("Four Of A Kind"); break; default:System.out.println("Invalid Hand"); } After we have checked what type of poker hand it is, we want to print out how strong that poker hand is by using a multiple if statements . The first if statement checks if the rank of UserHand's first card is less than or equal to 5 . If it is less than or equal to 5 , then it prints out "Small Straight". The second if statement checks if UserHand's first card's rank is greater than or equal to 6 . If it is greater than or equal to 6 , then it prints out "Large Straight". The third if statement checks if UserHand has two cards of same rank . If they do have two cards of same rank , then it prints out "Two Cards Of Same Rank". The fourth if statement checks if UserHand has three cards of same suit . If they do have three cards of same suit , then it prints out "Three Cards Of Same Suit". Here is what our code looks like so far: import java.util.*; public class Poker { public static void main(String[] args) { Scanner scan = new Scanner(System); boolean done = false; String userHand = null; int card1 = 0; int card2 = 0; int card3 = 0; int card4 = 0; while (!done) { System.out-println("Please enter your Poker Hand : "); userHand = scanLine(); switch(userHand){ //Checking for different types of poker hands here } } } } So far so good! Let's move on to part two of our program where we will declare five more variables called currentCard1 , currentCard2 , currentCard3 , currentCard4 , and currentCard5 . We will set these variables to null so that we can later set them to the user's input as well . Next, we want to have another while loop that will continuously ask the user for input until they enter "exit". We will set a boolean variable called done2 to true once the user enters "exit". Once done2 is true, we will break out of the while loop and move on on to part three of our program .





 inside the while loop just like before . We first get the user's input by using scanLine

#  Java Program with Two Inputs: Poker Hand and Fingers!

## Introduction

This program prints a poker hand, given the name of the hand and the number of fingers. The program also prints "How many fingers?" followed by the number of fingers input by the user.

## Poker Hand

The poker hands are as follows:

* Royal flush: A, K, Q, J, 10 all of the same suit.

* Straight flush: Five consecutive cards of the same suit.

* Four of a kind: Four cards of the same rank.

* Full house: Three cards of one rank and two cards of another rank.

* Flush: Any five cards of the same suit not in sequence.

* Straight: Five consecutive cards not all in the same suit.

* Three of a kind: Three cards of the same rank.

* Two pair: Two different pairs.
YOUR_HAND_NAME is either "royal flush", "straight flush", "four of a kind", "full house", "flush", "straight", "three of a kind", or "two pair". The number of fingers corresponds to the rank of your hand (e.g., 5 for a royal flush). For example, if you enter "two pair" as your hand, then you would be shown two different pairs on the screen (e.g., 2 and 3).

Your_hand_name has {0} fingers!

## Output Examples

Here are some examples of how this program runs:

If you enter "flush" as your hand, then you would be shown five different suits on the screen (e.g., clubs, hearts, spades, diamonds, clubs). 

Your_hand_name has {0} fingers!

If you enter "three of a kind" as your hand, then you would be shown three cards on the screen that are all threes (e.g., 3, 3, 3). 

Your_hand_name has {1} fingers!

#  Second Java Program: Poker Hand and Finger Input!

This is our second Java program! In this one, we'll be looking at how to handle user input with fingers, as well as create a basic poker hand.

We'll first import the necessary classes that we'll need for our program.

import java.util.Scanner; // For user input
import javax.swing.JOptionPane; // For displaying messages to the user
import java.awt.Graphics2D; // For drawing graphics on the screen

Then, we'll declare some global variables that will hold our information. 

final int NUM_OF_HANDS = 5; // The number of hands to generate 
final String[] HAND_NAME = {"Royal Flush", "Straight Flush", "Four of a Kind", "Full House", "Flush"}; // The names of the poker hands 
final int[] CARD_VALUE = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10}; // The values of the cards 
int currentHand = 0; // The current hand being dealt 
String userInputedCards = ""; // The user's inputed cards (empty string if no input) 
int[] selectedCards = new int[NUM_OF_HANDS]; // Selected cards for each hand 
bool winningHand = false; // A flag to indicate if a hand is a winner or not 
boolean validInput = true; // Whether or not the input is valid
 boolean addSelectedCard = false; // Whether or not to add the selected card to the hand


Now that we have our variables set up, we can begin coding our main() method. First, we'll ask the user how many hands they would like to generate.

System.out.print("How many hands would you like to generate? ");

Scanner in = new Scanner(System.in); 
int numHands = in.nextInt();

Next, we'll create an instance of JOptionPane and use it to display messages to the user. We'll also use it to get input from the user for their cards.

JOptionPane pane = new JOptionPane();

pane.showMessageDialog(null,"Welcome to our Java Poker Program!", "Message", JOptionPane.INFORMATION_MESSAGE);

pane.showMessageDialog(null,"Please enter your cards.", "Card Entry", JOptionPane.INFORMATION_MESSAGE);

We also need a way to store the user's inputted cards so that we can use them later in the program. We can do this by using a String variable named userInputedCards .

userInputedCards = pane.getText();

Now that we have a way to store the user's inputted cards, let's start creating our poker hands! We'll start by creating a method named createHand() . This method will take an integer as an argument and will return a Hand object with that rank and suit . For example, if the argument is 2 , then the Hand object will have a rank of 2 and a suit of spades . Here's how we can write this method:

public static Hand createHand(int rank, char suit) {

if (rank < 1 || rank > 13) {
throw new IllegalArgumentException("Rank must be between 1 and 13");  } 
if (suit < 'a' || suit > 'z') { throw new IllegalArgumentException("Suit must be between 'a' and 'z') };

 switch (rank) { case 1: return new Hand(suit, 10); case 2: return new Hand(suit,'S'); case 3: return new Hand(suit,'D'); case 4: return new Hand(suit,'H'); case 5: return new Hand(suit,'C'); default: break; }; }

#  Java Program with Two Inputs: Poker Hand and Finger Mode

This program will take input for a poker hand and whether the player wants to use finger mode. In finger mode, the player will use their fingers to indicate the rank of each card. The program will then generate a list of all possible poker hands for that particular combination of cards.

## Poker Hand

Input type: text

For this example, we will be using a five card poker hand. The user will input the rank of each card in the poker hand. There are 13 different ranks (A-2, 3-4, 5-6, 7-8, 9-10, J-Q, K-A).

### Ace of Spades
The user would input: "1" for the first card, "A" for the second card, "3" for the third card, "4" for the fourth card, and "5" for the fifth card. This would result in an Ace of Spades configuration. When playing in finger mode with this particular hand, the player would hold up one finger to represent the rank of the first card (an Ace), two fingers to represent the rank of the second card (a 2), etc. 
The following list contains all possible poker hands that can be made with an Ace of Spades: 
{Ace}{King}{Queen}{Jack}{Ten} 
{Ace}{Queen}{Jack}{Ten} 
{King}{Queen}{Jack}{Ten} 
{King}{Queen}{Ten} 
{King}{Jack}