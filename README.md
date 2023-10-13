using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Cansole_Calculator
{
    internal class Program
    {
        static void Main(string[] args)
        {
            double firstnum;
            double secondnum;
            double answer;
            string ops;

            Console.WriteLine("\t\t\t Simple Calculator\n");

            Console.WriteLine("\t\t\t ---------------- \n");

            Console.WriteLine("\t\t\t Enter First Number\n");
            firstnum = Double.Parse(Console.ReadLine());

            Console.WriteLine("\t\t\t Select an operator (+,-,*,/,%,^) \n");
            ops = Console.ReadLine();

            Console.WriteLine("\t\t\t Enter Second Number\n");
            secondnum = Double.Parse(Console.ReadLine());

            if(ops == "+")
            {
                answer = firstnum + secondnum;
                Console.Write("\n\t\t\t" + answer);
            }
            if (ops == "-")
            {
                answer = firstnum - secondnum;
                Console.Write("\n\t\t\t" + answer);
            }
            if (ops == "*")
            {
                answer = firstnum * secondnum;
                Console.Write("\n\t\t\t" + answer);
            }
            if (ops == "/")
            {
                answer = firstnum / secondnum;
                Console.Write("\n\t\t\t" + answer);
            }
            if (ops == "%")
            {
                answer = firstnum % secondnum;
                Console.Write("\n\t\t\t" + answer);
            }
            Console.Write("\n\n\t\t\t" + "Press any key to exit....\n");
            Console.ReadKey();
        }
    }
}
