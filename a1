using Microsoft.Win32.SafeHandles;
using System;
using System.ComponentModel.DataAnnotations;
using System.Dynamic;
using System.Linq;
using System.Security.Cryptography;
using System.Security.Cryptography.X509Certificates;

namespace TrackTimes
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Welcome to the TrackTimes program");
            Console.WriteLine("This was written in C#");
            Console.WriteLine("Enter com to start. When you are finished entering personal records type pr to list them.");
            Console.WriteLine("Type specified race, then your time to set a record.");

            var x = Console.ReadLine();
            if (x is "com")
            {
                Console.WriteLine("Reading values...");
                Console.WriteLine("Enter race, then time");
                string[] times = { "one", "two", "three", "four" };
                var cmd = Console.ReadLine();
                if (cmd is "mile")
                {
                    Console.WriteLine("Mile selected");
                    var mile = Console.ReadLine();
                    if (mile is string)
                    {
                        Console.WriteLine(mile, "is now your mile record");
                        times[0] = mile;
                        Console.ReadLine();
                        return;
                    }
                    else
                    {
                        Console.WriteLine("Error, you can only enter a number value");
                        Console.ReadLine();
                        return;
                    }
                }
                if (cmd is "2 mile")
                {
                    Console.WriteLine("2 Mile selected");
                    var twomile = Console.ReadLine();
                    if (twomile is string)
                    {
                        Console.WriteLine(twomile, "is now your mile record");
                        times[1] = twomile;
                        Console.ReadLine();
                        return;
                    }
                    else
                    {
                        Console.WriteLine("Error, you can only enter a number value");
                        Console.ReadLine();
                        return;
                    }
                }
                if (cmd is "5k")
                {
                    Console.WriteLine("5k selected");
                    var fivek = Console.ReadLine();
                    if (fivek is string)
                    {
                        Console.WriteLine(fivek, "is now your mile record");
                        times[2] = fivek;
                    }
                    else
                    {
                        Console.WriteLine("Error, you can only enter a number value");
                        return;
                    }
                }
                if (cmd is "10k")
                {
                    Console.WriteLine("10k selected");
                    var tenk = Console.ReadLine();
                    if (tenk is int)
                    {
                        Console.WriteLine(tenk, "is now your mile record");
                        times[3] = tenk;
                        Console.ReadLine();
                        return;
                    }
                    else
                    {
                        Console.WriteLine("Error, you can only enter a number value");
                        Console.ReadLine();
                        return;
                    }
                }
                if (cmd is "help")
                {
                    Console.WriteLine("Enter specified race. Console will notify when race is selected, then enter your time and console will read it back to you");
                    Console.ReadLine();
                    return;
                }

                if (cmd is "pr")
                {
                    Console.WriteLine(times);
                    return;
                }

            }
            Console.WriteLine("Enter specified race to see my PR.");
            var y = Console.ReadLine();
            if (y is string)
            {
                if (y is "mile")
                {
                    Console.WriteLine("5:19");
                    return;
                }
                if (y is "2k")
                {
                    Console.WriteLine("7:07");
                    return;
                }
                if (y is "2 mile") 
                {
                    Console.WriteLine("12:04");
                    return;
                }
                if (y is "5k")
                {
                    Console.WriteLine("20:22");
                    return;
                }
                if (y is "10k")
                {
                    Console.WriteLine("46:51");
                    return;
                }
            }
            


        }
    }
}
