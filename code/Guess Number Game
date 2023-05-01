using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace NumberGuesser
{
    internal class Program
    {
        static void Main(string[] args)
        {

            //set app vars
            string appName = "Number Guesser";
            string appVersion = "1.0.0";
            string appAuthor = "Anand";

            //Change the text color
            Console.ForegroundColor = ConsoleColor.Green;
            Console.WriteLine("{0}:Version {1} by {2} ", appName, appVersion, appAuthor);

            //Reset the color
            Console.ResetColor();

            //Ask the username
            Console.WriteLine("What is your name?");
            //Taking the name of the user
            string name = Console.ReadLine();

            Console.WriteLine("Hello {0}, let's play the game...", name);
            while (true)
            {
                //Init the correct number

                //int correctNumber = 7;

                //Random object creation
                Random random = new Random();

                //Taking the random number for the correct answer
                int correctNumber = random.Next(1, 10);

                //Init guess var
                int guess = 0;

                Console.WriteLine("Guess a number between 1 and 10");

                //While guess is not correct
                while (guess != correctNumber)
                {
                    string input = Console.ReadLine();

                    //Make sure it's a number
                    if (!int.TryParse(input, out guess))
                    {
                        //Change to red color if the user enter anything other than the integer
                        Console.ForegroundColor = ConsoleColor.Red;

                        //Display the message
                        Console.WriteLine("Please enter the number");

                        //Reset the color
                        Console.ResetColor();

                        //keep going
                        continue;
                    }
                    //converting the string input to int
                    guess = Convert.ToInt32(input);

                    //Match guess to correct number 
                    if (guess != correctNumber)
                    {
                        //Change to red color
                        Console.ForegroundColor = ConsoleColor.Red;

                        //Display Message
                        Console.WriteLine("Wrong number, please try again");

                        //Reset the color
                        Console.ResetColor();
                    }
                }
                //Change the output of the color if answer is correct
                Console.ForegroundColor = ConsoleColor.Yellow;

                //Display the message
                Console.WriteLine("You are correct!!!");

                //Reset the color 
                Console.ResetColor();

                //Ask if they want to continue
                Console.WriteLine("You want to play? Y or N");
                string ans = Console.ReadLine().ToUpper();

                if (ans == "Y")
                {
                    continue;
                }
                else if (ans == "N")
                {
                    return;

                }
                else
                {
                    return;
                }

            }
        }
    }
}
