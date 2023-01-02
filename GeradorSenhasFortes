using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;

namespace PasswordGenerator
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Insira o tamanho desejado para a senha:");
            string input = Console.ReadLine();

            //Verifique se o input é um número inteiro válido
            if (!int.TryParse(input, out int length))
            {
                Console.WriteLine("Erro: Tamanho da senha inválido.");
                return;
            }

            // Use a classe Random para gerar uma senha aleatória
            Random random = new Random();
            const string chars = "ABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789";
            string password = new string(Enumerable.Repeat(chars, length)
              .Select(s => s[random.Next(s.Length)]).ToArray());

            Console.WriteLine("Sua senha gerada aleatoriamente é: " + password);
        }
    }
}
