# Hesap-Makinesi
using System.ComponentModel.Design;

internal class Program
{
    private static void Main(string[] args)
    {
        Console.WriteLine("basit bir C# hesap makinesi");

        string islem;
        double num1, num2, sonuc=0;

        Console.WriteLine("bir sayı giriniz");
        num1=Convert.ToDouble(Console.ReadLine());

        Console.WriteLine("bir sayı giriniz");
        num2 =Convert.ToDouble(Console.ReadLine());   

        Console.WriteLine("işlem seçiniz: [ + | - | * | / | ] çıkış yapmak için boş geçiniz");
        islem = (Console.ReadLine());
        
           switch (islem)
            {
                case "+":
                    sonuc = num1 + num2;
                    break; 

                case "-":
                    sonuc = num1 - num2;
                    break;
                case "*":
                    sonuc = num1 * num2;
                    break;
                case "/":
                    sonuc = num1 / num2;
                    break;
                default:
                    break;
            }
            Console.WriteLine("sonuc: " + sonuc);
    

    }
}
