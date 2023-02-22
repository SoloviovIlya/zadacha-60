//Сформируйте трёхмерный массив из неповторяющихся двузначных чисел. Напишите программу, которая будет построчно выводить массив, добавляя индексы каждого элемента.
//Массив размером 2 x 2 x 2
//66(0,0,0) 25(0,1,0)
//34(1,0,0) 41(1,1,0)
//27(0,0,1) 90(0,1,1)
//26(1,0,1) 55(1,1,1)

Console.WriteLine("Введите размерность трёхмерного массива: ");

int m = Convert.ToInt32(Console.ReadLine());

int n = Convert.ToInt32(Console.ReadLine());

int k = Convert.ToInt32(Console.ReadLine());

int[, ,] a = new int[m,n, k];

Console.WriteLine("Введите элементы массива: ");

for (int i = 0; i < m;i++)

{

    for (int j =0; j<n; j++)
    
    {
    
        for (int l =0; l<k; l++)
        {
        a[i,j,l] = Convert.ToInt32(Console.ReadLine());
    }
    
    }
    
}

for (int i = 0; i < m;i++)

{

    for (int j =0; j<n; j++)
    
    {
    
        for (int l =0; l<k; l++)
        {
        Console.WriteLine($"{a[i,j,l]} ({i},{j},{l})");
    }
    
    }
    
    Console.Write(Environment.NewLine + Environment.NewLine);
    
}
