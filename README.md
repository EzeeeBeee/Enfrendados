#include <iostream>
using namespace std;

void mostrarTitulo();
void PreguntoCuantosJugadoresSon();
void MostrarMenu();
string PreguntoNombreJugador1();
string PreguntoNombreJugador2();
string PreguntoNombreJugador3();
string PreguntoNombreJugador4();


string PreguntoNombreJugador1 (){
  string jugador1;
  cout<< "Ingresar nombre de jugador1"<<endl;
  cin>>jugador1;
     system ("cls");
  return "Bienvenido/a "+jugador1+"!";

}
string PreguntoNombreJugador2 (){
    string jugador2;
  cout<< "Ingresar nombre de jugador2"<<endl;
  cin>>jugador2;
  system ("cls");
  return "Bienvenido/a "+jugador2+ "!";
}

string PreguntoNombreJugador3 (){
    string jugador3;
  cout<< "Ingresar nombre de jugador3"<<endl;
  cin>>jugador3;
  system ("cls");
  return "Bienvenido/a "+jugador3+ "!";
 }

string PreguntoNombreJugador4 (){
    string jugador4;
  cout<< "Ingresar nombre de jugador4"<<endl;
  cin>>jugador4;
  system ("cls");
  return "Bienvenido/a "+jugador4+ "!";
 }


void mostrarTitulo() {
    cout<<endl<<
"     _______   ____________  _______   ______  ___    ____  ____  _____"<<endl<<
"    /____ / |  // ____/ __ \/ ____/ | / / __ \/   |  / __ \/ __ \/ ___ "<<endl<<
"   / __/ /  |/ / /_  / /_/ / __/ /  |/ / / / / /| | / / / / / / /\__ \ "<<endl<<
"  / /___/ /|  / __/ / _  _/ /___/ /|  / /_/ / ___ |/ /_/ / /_/ /___/ /"<<endl<<
" /_____/_/ |_/_/   /_/ |_/_____/_/ |_/_____/_/  |_/_____/\____//____/"<<endl<<endl;
system ("pause");
 system ("cls");
}



    // system ("pause");  "Presiona una tecla para continuar" // system ("cls"); paralimpiar pantalla


 void PreguntoCuantosJugadoresSon() {
     int opcion;

    do {

   cout << " 1 -- 2 Jugadores  (Eazy) ";
   cout << endl;
   cout << "2 -- 3 Jugadores  (Medium)";
   cout << endl;
   cout << "3 -- 4 Jugadores  (Hardcore) ";
   cout << endl;


    cin >> opcion;

    switch (opcion) {

case 1:
    cout<<PreguntoNombreJugador1()<<endl;
    cout<<PreguntoNombreJugador2()<<endl;
    break;

case 2:
   cout<<PreguntoNombreJugador1()<<endl;
   cout<<PreguntoNombreJugador2()<<endl;
   cout<<PreguntoNombreJugador3()<<endl;
    break;

case 3:
  cout<<PreguntoNombreJugador1()<<endl;
  cout<<PreguntoNombreJugador2()<<endl;
  cout<<PreguntoNombreJugador3()<<endl;
  cout<<PreguntoNombreJugador4()<<endl;
    break;
    }


 } while (opcion != 1 && opcion != 2 && opcion  != 3);
 }



void MostrarMenu () {
   int op;

    do {

   cout << "1 - JUGAR";
   cout << endl;
   cout << "2 - ESTADÍSTICAS";
   cout << endl;
   cout << "3 - CRÉDITOS";
   cout << endl;
   cout << "-----------------";
   cout << endl;
   cout << "4 - SALIR";
   cout << endl;

  cin>>  op;


    switch (op) {
  case 1:
   PreguntoCuantosJugadoresSon() ;
    break;
  case 2:
      cout<< "Todavia no esta configurado ";
    //  MuestroEstadisticas();
    break;
     case 3:
         cout<< "Todavia no esta configurado ";
    // Creditos();
    break;
     case 4:
         cout<< "Todavia no esta configurado";
   // SalirDelJuego();
    break;
     default:
        cout<< "Error 404, Intente de nuevo con otro numero de opcion... "<<endl;
}

}   while (op !=4);

 }



// _____________________________________________________________________________________


int main (){



 mostrarTitulo();

 MostrarMenu();



/*
cout<<endl<<PreguntoNombreJugador1();

// system ("cls");
cout<<endl<<PreguntoNombreJugador2()<<endl;

*/














    return 0;
}
