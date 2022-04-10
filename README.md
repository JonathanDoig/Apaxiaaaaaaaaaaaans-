/*Jonathan Doig
 * 4/9/2022
 * code to remove repetition of a letter
 */
using System;

namespace NameShortenator
{
    class Program
    {
        static void Main(string[] args)
        {
            String longname = Console.ReadLine();
            String shortname = "";

            char letter = ' ';

            foreach(char x in longname)
            {
                if(x == letter)
                {
                    continue;
                }
                else
                {
                    letter = x;
                    shortname += x;
                }
            }
            Console.Write(shortname);
        }
    }
}
