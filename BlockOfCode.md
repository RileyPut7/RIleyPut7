# Here is a block of code that I wrote for my 2040 INFOTTC class.
_This Code will produce a text document with a title and content after completing the requried operations._

using System;

using System.IO;

namespace DocumentApplication
{

    class Document
    {

        static void Main(string[] args)
        {

            try
            {

                Console.WriteLine("Document");

                Console.WriteLine("Enter Document Title:");

                string name = Console.ReadLine();

                Console.WriteLine("Enter Document Content:");

                string content = Console.ReadLine();

                string filename = name + ".txt";

                string path = Environment.CurrentDirectory + "/" + filename;

                if (!File.Exists(path))

                {

                    File.WriteAllText(path, content);

                }

                Console.WriteLine(filename + " was successfully saved. The document contains " + content.Length + " characters");

            }

            catch (Exception e)

            {

                Console.WriteLine(e +" The file contains an exception" );

            }

        }

    }

}

Back to Home --> [README.md](https://github.com/RileyPut7/RIleyPut7/edit/master/README.md)
