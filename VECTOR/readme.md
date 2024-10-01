# TITULO 1
## TITULO 2
### TITULO 3
#### TITULO 4

* uno
* dos
* tres

1. punto 1
2. punto 2
3. punto 3

**NEGRITAS** 
_italica:

**italica negritas**

```C++
#include <iostream>
#include <vector>
using namespace std;

void imprime(vector<int> v)
{
    for (auto elemento : v)
    {
        cout << elemento << " , ";
    }
    cout << endl;
    system("pause");
    system("cls");
}

int main()
{

    vector <int> v;

    // Llenar vector con 0, 5 veces

    v.assign(5, 0);
    imprime(v);
    system("pause");
    system("cls");

    // Inserta 15 en la ultima posicion

    v.push_back(15);
    imprime(v);

    // Quitar el ultimo elemento

    v.pop_back();
    imprime(v);

    // Inserta un 5 al principio del vector

    v.insert(v.begin(), 5);
    imprime(v);

    // Borra el primer elemento del vector
    v.erase(v.begin());
    imprime(v);

    // Emplace() inserta 25 al principio

    v.emplace(v.begin(), 25);
    imprime(v);

    // emplace_back() colocar 20 al final

    v.emplace_back(20);
    imprime(v);

    // Borrar completamente el vector

    v.clear();
    imprime(v);

    // Swap entre dos vectores

    vector<int> v1, v2;
    v1.push_back(1);
    v1.push_back(2);
    v2.push_back(3);
    v2.push_back(4);
    v1.swap(v2);
    imprime(v1);
    imprime(v2);
}

```



