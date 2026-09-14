# c-_1


using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {

            /*Futás-Km-Összegző feladat!
                1. Feladat: Kérje be a felhasználótól a nevét, és mentse el egy string típusú változóba!
                2. Feladat: A bekérés után írja ki: "Rendben *név*! Hányszor futott a héten: ", és mentse el ezt egy int típusú változóba!
                3. Feladat: Csináljon egy int típusú listát, majd egy for ciklusban írja meg, hogy számolja össze a naponta elért km-ek értékét a keletkezett listába.
                A bekérésekor írja ki mindig, hanyadik napnál jár az illető!
                4. Feladat: Írjon egy olyan ciklust, ami megszámolja hány km-t futott összesen a napok alatt!
             
             
             */
            #region 1. Feladat
            Console.Write("Üdvözlöm, hogy hívhatom Önt: ");
            string nev = Console.ReadLine();
            #endregion
            #region 2. Feladat
            Console.WriteLine($"Rendben {nev}! Hányszor futott a héten: ");
            int szam = Convert.ToInt32(Console.ReadLine());
            #endregion
            #region 3. Feladat
            List<int> lista = new List<int>();
            for (int i = 0; i < szam; i++)
            {
                Console.Write($"Mennyi km-t futott {i + 1}. napon: ");
                lista.Add(Convert.ToInt32(Console.ReadLine()));

            }
            #endregion
            #region 4. Feladat
            int osszeg = 0;
            for (int i = 0; i < lista.Count; i++)
            {
                osszeg += lista[i];
            }
            Console.WriteLine($"Összes km: {osszeg}");
            #endregion



        }
    }
}
