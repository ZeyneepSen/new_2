static void Main(string[] args)
        {
            Console.Write("Metni Gir: ");
            string metin =Console.ReadLine();
            string yeniMetin = "";
            foreach (char c in metin)
            {
                if (Char.IsUpper(c))
                    yeniMetin += Char.ToLower(c);
                else
                    yeniMetin += Char.ToUpper(c);
            }
            
            Console.WriteLine(yeniMetin);
            Console.ReadLine();
        }