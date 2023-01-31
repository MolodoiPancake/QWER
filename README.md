# string[] FirstArray = new string[6] {"1234", "2", "hello", "world", ":3", "Aboba"};
string[] SecondArray = new string[FirstArray.Length];
void SecondArrayWithIF(string[] FirstArray, string[] array2)
{
    int count = 0;
    for (int i = 0; i < FirstArray.Length; i++)
    {
    if(FirstArray[i].Length <= 3)
        {
        SecondArray[count] = FirstArray[i];
        count++;
        }
    }
}
void PrintArray(string[] array)
{
    for (int i = 0; i < array.Length; i++)
    {
        Console.Write($"{array[i]} ");
    }
    Console.WriteLine();
}
Console.Clear();
SecondArrayWithIF(FirstArray, SecondArray);
PrintArray(SecondArray);

## 
# Написать программу, которая из имеющегося массива строк формирует массив из строк, длина которых меньше либо равна 3 символа. Первоначальный массив можно ввести с клавиатуры, либо задать на старте выполнения алгоритма. При решение не рекомендуется пользоваться коллекциями, лучше обойтись исключительно массивами 

## Описание алгоритма решения

# Создаем два массива - изначальный(FirstArray) и конечный такой же длиный(SeconsdArray). Потом проверяется условие через цикл "for" (FirstArray[i].Length <= 3) если да, то элемент FirstArray  заносится в count элемент SeconsdArray. После присвоения увеличивается переменная count на 1 и возвращается к циклу for в котором i увеличивается на 1. И так проверяется до конца.
