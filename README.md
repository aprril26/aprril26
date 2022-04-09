using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace CalculatorConsoleApp
{
    internal class Program
    {
        static void Main(int[] args)
        {
			Console.Title = "Aplikasi Calculator";

			// int a = 10; // declarasi variabel a, dg nilai awal 10;
			// int b = 6; // declarasi variabel b, dg nilai awal 6;

			Console.Write("Inputkan nilai a=");
			int a = int.Parse(Console.Readline()); // proses casting

			Console.Write("Inputkan nilai b=");
			int b = Convert.ToInt32(Console.Readline()); // proses casting

			Console.Writeline(); // tambahkan baris kosong

			Console.Writeline("Hasil penambahan " + a + " + " + b + " = " + penambahan(a, b));
			Console.Writeline("Hasil pengurangan {0}-{1}={2}", a, b, pengurangan(a, b));
			Console.Writeline("Hasil perkalian {0}*{1}={2}", a, b, perkalian(a, b));
			Console.Writeline("Hasil pembagian {0}/{1}={2}", a, b, pembagian(a, b));

			Console.Writeline("\nTekan sembarang key untuk keluar");
			Console.Readkey();
		}
		static int penambahan(int a, int b)
		{
			return a + b;
		}
		static int pengurangan(int a, int b)
		{
			return a - b;
		}
		static int perkalian(int a, int b)
		{
			return a * b;
		}
		static int pembagian(int a, int b)
		{
			return a / b;
		}
}
