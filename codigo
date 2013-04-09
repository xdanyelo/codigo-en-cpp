#include <iostream>
#include <iomanip>

using namespace std;

const int tamanioArreglo = 10;
void ordenamiento(int *const, const int);
void intercambio(int *const, int *const);

int main(int argc, char **argv) {

	int arregloA[tamanioArreglo] = {67, 54, 34, 22, 12, 15, 4, 6, 78, 48};
	ordenamiento(arregloA, tamanioArreglo);

	for(int contador = 0; contador < tamanioArreglo; contador++)
		cout << setw(5) << arregloA[contador];
}

void ordenamiento(int *const arregloB, const int tamanioArreglo){
	int menor;
	for(int i = 0; i < tamanioArreglo - 1; i++){
		menor = i;
		for(int subindice = i + 1; subindice < tamanioArreglo; subindice++)
			if(arregloB[menor] > arregloB[subindice])
				menor = subindice;

		intercambio(&arregloB[i], &arregloB[menor]);
	}
}
void intercambio(int *const elemento1Ptr, int *const elemento2Ptr){
	int temporal = *elemento1Ptr;
	*elemento1Ptr = *elemento2Ptr;
	*elemento2Ptr = temporal;
}
