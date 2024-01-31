Лекция 6. Домашнее задание.

// Задача 1: Задайте двумерный массив символов (тип char [,]). Создать строку из символов этого массива.


char[,] array = new char[,]
{
    {'a', 'b', 'c'},
    {'d', 'e', 'f'},
    {'g', 'h', 'i'}
};

string result = string.Empty;

for (int i = 0; i < array.GetLength(0); i++)
{
    for (int j = 0; j < array.GetLength(1); j++)
    {
        result += array[i, j];
    }
}

Console.WriteLine(result);


// Задайте строку, содержащую латинские буквы в обоих регистрах. Сформируйте строку, в которой все заглавные буквы заменены на строчные.

Console.WriteLine("Введите строку:");
string str = Console.ReadLine();
string result = str.ToLower();
Console.WriteLine("Результат: " + result);


// Задайте произвольную строку. Выясните, является ли она палиндромом.

Console.WriteLine("Введите слово:");
string str = Console.ReadLine();
{
            char[] arr = { 'а', 'я',};
            if (IsPalindrom(arr))
                Console.WriteLine("Палиндром");
            else
                Console.WriteLine("Не палиндром");
        }
 
        static bool IsPalindrom(char[] word)
        {
            for (int i = 0; i < word.Length / 2; i++)
                if (word[i] != word[word.Length - 1 - i])
                    return false;
            return true;
        }
