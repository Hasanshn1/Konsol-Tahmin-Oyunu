# Konsol-Tahmin-Oyunu

using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace OdevTahmin
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine(" Oyunumuza Hoşgeldiniz :) ");
            Console.WriteLine(" Başlamak için seviye seçiniz: \n 1-Kolay Seviye \n 2-Orta Seviye \n 3-Zor Seviye ");
            string seviye = Console.ReadLine();
            

            if (seviye == "1")
            {
                Console.WriteLine("Bu oyunda 6 hakkınız bulunmaktadır.");
                int hak = 6;
                Random rnd = new Random();
                int sayi = rnd.Next(10);

                for (int i = 0; i < 6; i++)
                {
                    Console.WriteLine("Bir sayı tahmin et: ");
                    int tahmin = int.Parse(Console.ReadLine());
                    if (sayi == tahmin)
                    {
                        Console.WriteLine("Tebrikler Bildiniz");
                        break;
                    }
                    else
                    {
                        hak--;
                        Console.WriteLine("Bilemediniz. Tekrar Deneyiniz \n Kalan hak: " + hak);
                        if (hak == 0)
                        {
                            Console.WriteLine("Hakkınız bitti!!");
                        }
                    }

                }
            }
            else if (seviye == "2")
            {
                Console.WriteLine("Bu oyunda 4 hakkınız bulunmaktadır.");
                int hak = 4;
                Random rnd = new Random();
                int sayi = rnd.Next(25);

                for (int i = 0; i < 4; i++)
                {
                    Console.WriteLine("Bir sayı tahmin et: ");
                    int tahmin = int.Parse(Console.ReadLine());
                    if (sayi == tahmin)
                    {
                        Console.WriteLine("Tebrikler Bildiniz");
                        break;
                    }
                    else
                    {
                        hak--;
                        Console.WriteLine("Bilemediniz. Tekrar Deneyiniz \n Kalan hak: " + hak);
                        if (hak == 0)
                        {
                            Console.WriteLine("Hakkınız bitti!!");
                        }
                    }

                }
            }
            else if (seviye == "3")
            {
                Console.WriteLine("Bu oyunda 2 hakkınız bulunmaktadır.");
                int hak = 2;
                Random rnd = new Random();
                int sayi = rnd.Next(50);

                for (int i = 0; i < 2; i++)
                {
                    Console.WriteLine("Bir sayı tahmin et: ");
                    int tahmin = int.Parse(Console.ReadLine());
                    if (sayi == tahmin)
                    {
                        Console.WriteLine("Tebrikler Bildiniz");
                        break;
                    }
                    else
                    {
                        hak--;
                        Console.WriteLine("Bilemediniz. Tekrar Deneyiniz \n Kalan hak: " + hak);
                        if (hak == 0)
                        {
                            Console.WriteLine("Hakkınız bitti!!");
                        }
                    }

                }
            }

            Console.ReadKey();
        }
    }
}
