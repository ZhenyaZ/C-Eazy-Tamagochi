# C-Eazy-Tamagochi
I wrote here such a tamagochi) Do not judge strictly, since I only study for 1 week C #
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace TamagochiTest
{
    class Animal
    {
        public static int count = 0;
        public Animal()
        {
            Input();
            
        }
        public void Input()
        {
            string inputName;
            int inputAge;
            int inputSila;
            int inputVin;
            Console.WriteLine("Input Name you pets: ");
            inputName = Convert.ToString(Console.ReadLine());
            Console.WriteLine("Input Age you pets: ");
            inputAge = Convert.ToInt32(Console.ReadLine());
            Console.WriteLine("Input Power you pets: ");
            inputSila = Convert.ToInt32(Console.ReadLine());
            Console.WriteLine("Input Stamina you pets: ");
            inputVin = Convert.ToInt32(Console.ReadLine());
            Console.WriteLine("Name your pets: " + inputName);
            Console.WriteLine("Age your pets: " + inputAge);
            Console.WriteLine("Power you pets: " + inputSila);
            Console.WriteLine("Stamina your pets: " + inputVin);
            count++;
        }
    }
    class Program
    {
        static void Main(string[] args)
        {
            Animal pets = new Animal();
            Console.WriteLine("Your pets: " + Animal.count);
            Console.ReadKey();
        }
    }
}
