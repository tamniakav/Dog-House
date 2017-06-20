using System;

namespace Dog_House
{
    class Program
    {
        static void Main(string[] args)
        {
            double a = double.Parse(Console.ReadLine());
            double b = double.Parse(Console.ReadLine());

            double leftRightSide = (a * (a / 2.00));
            leftRightSide *= 2;
            double backQuad = (a / 2.00) * (a / 2.00);
            double backTriangle = (a / 2.00 * (b - a / 2.00));
            backTriangle /= 2.00;
            double backSide = backTriangle + backQuad;
            double enter = (a / 5.00) * (a / 5.00);
            double frontSide = backSide - enter;
            double sideAria = leftRightSide + backSide + frontSide;
            double greenColour = sideAria / 3.00;

            double roofAria = a * (a / 2.0);
            roofAria *= 2;
            double redColour = roofAria / 5.00;

            Console.WriteLine($"{greenColour:f2}");
            Console.WriteLine($"{redColour:f2}");
        }
    }
}
