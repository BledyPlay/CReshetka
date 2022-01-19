using System;

namespace CSharp
{
    class Program
    { 
        static void Main(string[] args)
        {
            int[,] matrix = new int[3, 3];
            Random rnd = new Random();

            //Заполнение матрицы рандомными числами от 0 до 99
            for (int i = 0; i < 3; i++)
            {
                for (int j = 0; j < 3; j++)
                {
                    matrix[i, j] = rnd.Next(0, 100);
                }
            }

            int[] nums = new int[3];

            //Заполнение массива элементами, стоящими на диагонали
            for (int i = 0; i < nums.Length; i++)
            {
                nums[i] = matrix[i, i];
            }

            //Сортировка пузырьком
            for (int i = 0; i < nums.Length; i++)
            {
                for (int j = i; j < nums.Length; j++)
                {
                    if (nums[i] < nums[j])
                    {
                        int temp = nums[i];
                        nums[i] = nums[j];
                        nums[j] = temp;
                    }
                }
            }

            //Вывод массива
            for (int i = 0; i < nums.Length; i++)
                Console.WriteLine(nums[i]);

        }
    }
}
