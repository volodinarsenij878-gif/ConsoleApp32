    using System;
    using System.Collections.Generic;
    using System.Linq;
    using System.Text;
    using System.Threading.Tasks;

    namespace Program32
    {
    internal class Program
    {
        static void Main(string[] args)
        {
            Console.Write("Введите строку для парсинга в int: ");
            string input = Console.ReadLine();

            if (int.TryParse(input, out int result))
            {
                Console.WriteLine($"Успешно! Получено число: {result}");
            }
            else
            {
                Console.WriteLine("Ошибка ввода: строка не является целым числом.");
            }
        }
    }
    }
