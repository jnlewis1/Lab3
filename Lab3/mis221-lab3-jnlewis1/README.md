// See https://aka.ms/new-console-template for more information
using System;

namespace Lab3

{
// Function: Two MIS TA’s had birthdays this week. Create an application that outputs a birthday message if it is a TA’s birthday. Use the information below to create your logic​
    // Monday is Joseph’s birthday
    // Thursday is Katie’s birthday​
// The application should collect the needed information from the user and display a message.​
    // Prompt user for day of week (Monday, Tuesday, etc.)​
    // Test if it is a TA’s birthday​
    // Display birthday message for correct TA​
    // If there are no birthdays on the day entered, the program should display “No birthdays today :(”

    class Program
    {

//Ref: Methods for Lab

    //GetDayOfWeek()​ 
        //Prompts user for day of week and returns value to main​​

    //BirthdayDecision(string day)​
        //Associates the day entered with the correct TA name and calls the SayHappyBirthday() method​

    // SayHappyBirthday(string name)​
        // Display a birthday message with the correct TA name
        
        
        static void Main(string[] args)
        {

            string day = GetDayOfWeek();
            string message = BirthdayDecision(day);
            SayHappyBirthday(message);

            //**
            // //static void GetDayOfWeek()​
            // //Prompt user for day
            // Console.WriteLine("Hi, welcome to the TA birthday simulator! Please enter a day of the week.");
            // //Read user input
            // string day = (Console.ReadLine());
            // //Return to main
            //**


            //**
             //Determine if it is a TA's bday
            // //public static void BirthdayDecision(string day)​
            // string bDayJoseph = "Monday";
            // string bDayKatie =  "Tuesday";
            // string name = "";

            // if(day == bDayJoseph) 
            // {
            //     name = "Joseph";
            //     //SayHappyBirthday(string name)​
            //     Console.WriteLine("Happy Birthday to " +  name + "!!!");
            // }
            // else if(day == bDayKatie) 
            // {
            //     name = "Katie";
            //     //SayHappyBirthday(string name)​
            //     Console.WriteLine("Happy Birthday to " +  name + "!!!");
            // }
            
            // else
            // {
            //     Console.WriteLine("No birthdays today :(");
            // }


            // //SayHappyBirthday(string name)​
            //     Console.WriteLine("Happy Birthday to " +  name + "!!!");

            //**
            }

         static string GetDayOfWeek()
         {
             //Prompt user for day
            Console.WriteLine("Hi, welcome to the TA birthday simulator! Please enter a day of the week.");
            //Read user input
            string day = (Console.ReadLine());
            return day;
         }

         static string BirthdayDecision(string day)
         {
             //Determine if it is a TA's bday
            //public static void BirthdayDecision(string day)​
            string bDayJoseph = "Monday";
            string bDayKatie =  "Thursday";
            string name = "";
            string message = "";

            if(day == bDayJoseph) 
            {
                name = "Joseph";
                //SayHappyBirthday(string name)​
                message = "Happy Birthday to " +  name + "!!!";
            }
            else if(day == bDayKatie) 
            {
                name = "Katie";
                //SayHappyBirthday(string name)​
                message = "Happy Birthday to " +  name + "!!!";
            }
            
            else
            {
                message = "No birthdays today :(";
                //Console.WriteLine("No birthdays today :(");
            }
            return message;
         }

        static string SayHappyBirthday(string message)
         {
             Console.WriteLine(message);
             return message;
         }


    }
}