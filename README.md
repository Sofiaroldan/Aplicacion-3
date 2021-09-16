# Aplicacion-3
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Aplicación_3
{
    class Program
    {
        static void Main(string[] args)
        {
            string Dirección = " Agenda.txt ";
            string Nombre = "";
            string Apellido = "";
            string Teléfono = "";

            string liena = "";

            for (int x = 0; x < 4; x++)
            {
                Console.WriteLine("Ingrese Nombre");
                Nombre = Console.ReadLine();
                Console.WriteLine("Ingrese Apellido");
                Apellido = Console.ReadLine();

                Console.WriteLine("Ingrese teléfono");
                Teléfono = Console.ReadLine();

                liena = Nombre + ";" + Apellido + ";" + Teléfono;
                EscribirArchivo(Dirección, liena);

            }

            static void EscribirArchivo(string ruta, string dato)
            {

                StreamWriter ar;
                ar = File.AppendText(ruta);
                ar.WriteLine(dato);
                ar.Close();

            }

            static void BuscarArchivo(string ruta, string Buscar)
            {
                string lineaAR = ;
                StreamReader ar;
                ar = File.OpenText(ruta);
                string Dirección = "Agenda.txt"; string Nombre = ""; string Apellido = ""; string Teléfono = "";
                cadena linea = "";
                for (int x = 0; x <4; x ++) {Console.WriteLine ("Ingrese Nombre"); Nombre = Console.ReadLine (); Console.WriteLine ("Ingrese Apellido"); Apellido = Console.ReadLine ();
                Console.WriteLine ("Ingrese teléfono"); Teléfono = Console.ReadLine ();
                linea = Nombre + ";" + Apellido + ";" + Teléfono; EscribirArchivo (Dirección, liena);
                }
                static void EscribirArchivo (string ruta, string dato) ;
                StreamWriter ar; ar = File.AppendText (ruta); ar.WriteLine (dato); ar.Close ();
                }
                ar = Archivo.OpenText (ruta);
                lineaAr = ar.ReadLine ();
                while (lineaAr! = pull) {string [] vec = lineaAr.Split (';'); if (vec [0]) == buscar || vec [1] == buscar) {Console.WriteLine ("Contacto encontrado:" + vec [0] + "-" + vec [0];
                } 
                lineaAr = ar.ReadLine ();
                while (lineaAr = null)
                { string[] vec = LineaAr.Split(";");
                    if (vec[0] == buscar || vec [1]== buscar)//&&
                    {
                        Console.WriteLine("Contacto encontrado: " + vec[0] + "--" + vec[1] + "--");
                    }
                    lineaAr = ar.Readline();





            }
        }
    }
}
