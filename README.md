# zadanie-[ConsoleApplication1.txt](https://github.com/Woberto/zadanie-/files/7375972/ConsoleApplication1.txt)
#include <iostream>
using namespace std;


int main()
{
    cout << "W65523" << endl;
    
    int liczba;
    cout << "wprowadz liczbe" << endl;
    cin >> liczba;
    if (liczba % 2 == 0) 
        cout << "wpisana liczba jest parzysta " << endl;
    else
        cout << "wpisana liczba jest nieparzysta" << endl;
    float g;
    float u;
    cout << "Podaj liczbe: ";
    cin >> g;
    cout << "Podaj liczbe: ";
    cin >> u;
    if (g > u)
        cout << g << " jest wieksze" << endl;
    else if (u > g)
        cout << u << " jest wieksze" << endl;
    float liczba1, liczba2, liczba3, liczba4;
    cout << " Podaj liczby\n";
    cin >> liczba1 >> liczba2 >> liczba3 >> liczba4;
    cin.ignore();
    float srednia;
    srednia = (liczba1 + liczba2 + liczba3 + liczba4) / 4;
    cout << " Srednia wynosi: " << srednia;
    
    int liczba33;
    int liczba22;
    int wynik = 0;
    do
    {
        cin.clear();
        cin.sync();
        cout << "Wynik: " << wynik << endl;
        cout << " Podaj 1 liczbe: ";
        cin >> liczba33;
        if (cin.good())
        {
            cout << "Podaj 2 liczbe: ";
            cin >> liczba22;
            if (cin.good())
            {
                cout << "[1] Dodawanie" << endl;
                cout << "[2] Odejmowanie" << endl;
                cout << "[3] Mnozenie" << endl;
                cout << "[4] Dzielenie" << endl;
                int co;
                cin >> co;
                switch (co)
                {
                case 1:
                    wynik = liczba33 + liczba22;
                    cout << liczba33 << " + " << liczba22 << " = " << wynik << endl;
                    break;
                case 2:
                    wynik = liczba33 - liczba22;
                    cout << liczba33 << " - " << liczba22 << " = " << wynik << endl;
                    break;
                case 3:
                    wynik = liczba33 * liczba22;
                    cout << liczba33 << " * " << liczba22 << " = " << wynik << endl;
                    break;
                case 4:
                    wynik = liczba33 / liczba22;
                    cout << liczba33 << " : " << liczba22 << " = " << wynik << endl;
                    cout << "Reszta: " << liczba33 % liczba22 << endl;
                    break;



                }
            }
        }


    } while( wynik > 0);
    return 0;
   
}
