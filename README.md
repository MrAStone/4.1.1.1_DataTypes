```
namespace _4._1._1._1_DataTypes
{
    internal class Program
    {
        struct Town
        {
            public string TownName;
            public int Population;
            public double Area;
            public string County;

            public Town(string tName, int tPop, double tArea, string tCounty)
            {
                this.TownName = tName;
                this.Population = tPop;
                this.Area = tArea;
                this.County = tCounty;
            }
        }
        static void Main(string[] args)
        {
            // integer
            int myNumber;
            myNumber = 10;
            int myNumber2 = 20;
            int myNumber3 = myNumber + myNumber2;

            //real - Different options, for float and decimal a digit needs to be added.
            // For simplicity, use double
            float myFloat = 0.3F; // low precision 6-9 digits
            double myDouble = 1.23456; // higer precision 15-17 digits
            decimal myDecimal = 1.31646m; // highest precision 28-29 digits

            // Boolean
            bool myBoolean = false;
            bool myBoolean2 = true;

            // character
            char myChar;
            myChar = 'a';
            char myChar2 = 'A';

            //• string.
            string myString = "This is a string";
            string myString2;
            myString2 = "";

            //•date/time 
            DateTime d = DateTime.Now; //the current date and time dd/mm/yyyy hh:mm:ss
            d = DateTime.Today; // the current date and time is set to 00:00:00
            Console.WriteLine(d);
            Console.WriteLine(d.Year);
            Console.WriteLine(d.Month);
            Console.WriteLine(d.Day);
            Console.WriteLine(d.Hour);
            Console.WriteLine(d.Minute);
            Console.WriteLine(d.Second);
            Console.WriteLine(d.Millisecond);


            //•pointer/reference 
            // Not safe in C# so we will not use.  points to memory address
            // int* ptr = &x;.
            // Console.WriteLine((int)ptr) // Displays the memory address
            // Console.WriteLine(*ptr) // Displays the value at the memory address.


            //•records (or equivalent)
            // In C# records are called structures (struct)
            // see top of code
            ////////     struct Town
            ////////{
            ////////    public string TownName;
            ////////    public int Population;
            ////////    public double Area;
            ////////    public string County;

            ////////    public Town(string tName, int tPop, double tArea, string tCounty)
            ////////    {
            ////////        this.TownName = tName;
            ////////        this.Population = tPop;
            ////////        this.Area = tArea;
            ////////        this.County = tCounty;
            ////////    }
            ////////}

            Town t;
            t.TownName = "Heckmondwike";
            t.Population = 12343;
            t.Area = 3.1414;
            t.County = "West Yorkshire";

            Town t2 = new Town("Batley", 4321, 3.123, "West Yorkshire");


            //•arrays (or equivalent).
            string[] strings = { "This", "Is", "An", "Array" };

            int[] nums = new int[10];
            nums[0] = 1;
            nums[1] = 2;
            //   nums[10] = -1; errors as there are only 10 locations
            Console.WriteLine(nums.Length);
        }
        }
}
```
