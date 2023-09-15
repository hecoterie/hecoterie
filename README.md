using System;

namespace ConsoleApp1
{
    class Program
    {
        struct Airport
        {
            public string code;
            public string name;
            public int dist1;
            public int dist2;
        }

        static Airport[] air = new Airport[5];

        static void Main(string[] args)
        {
            air[0].code = "JFK";
            air[0].name = "John F Kennedy International";
            air[0].dist1 = 5326;
            air[0].dist2 = 5486;
            air[1].code = "ORY";
            air[1].name = "Paris-Orly";
            air[1].dist1 = 629;
            air[1].dist2 = 379;
            air[2].code = "MAD";
            air[2].name = "Adolfo Suarez Madrid Barajas";
            air[2].dist1 = 1428;
            air[2].dist2 = 1151;
            air[3].code = "AMS";
            air[3].name = "Amsterdan Schipol";
            air[3].dist1 = 526;
            air[3].dist2 = 489;
            air[4].code = "CAI";
            air[4].name = "Cairo international";
            air[4].dist1 = 3779;
            air[4].dist2 = 3584;

            menu();
        }
       
        static void menu()
        {
            Console.WriteLine("Select the number from the following options:");
            Console.WriteLine("1 - Enter Airport details");
            Console.WriteLine("2 - Enter flight details");
            Console.WriteLine("3 - Enter price plan and calculate profit");
            Console.WriteLine("4 - Clear Data");
            Console.WriteLine("5 - Quit");
            int option = Convert.ToInt32(Console.ReadLine());

            if( option == 1)
            {
                option1();
            }
            if (option == 2)
            {
                option2();
            }
            if (option == 3)
            {
                option3();
            }
            if (option == 4)
            {
                option4();
            }
            if (option == 5)
            {
                option5();
            }



        }
    }
}


