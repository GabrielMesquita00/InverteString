# InverteString
Escreva um programa que inverta os caracteres de um string

----------------

private static void Main(string[] args)
    {
        Console.WriteLine("Digite uma frase ou palavra: ");
        string palavra = Console.ReadLine();

        string palavraContraria = Inversao(palavra); // chama função de inversão de palavra

        Console.WriteLine("\nPalavra normal: " + palavra);
        Console.WriteLine("Palavra invertida: " + palavraContraria);

        Console.ReadLine();

    }

    static string Inversao(string str)
    {
        string invertida = ""; // aramazenamento da palavra invertida

        for (int i = str.Length - 1; i >= 0; i--) // percorre a string da última posição até a primeira
        {
            invertida = invertida + str[i]; // e adiciona cada caractere à string invertida 

        }
        return invertida;
    }
