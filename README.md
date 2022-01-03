# pirma uzduotis https://leetcode.com/problems/length-of-last-word/ Paskutinio zodzio ilgis.

#include <iostream>
#include <string>
using namespace std;

int main() {


	string tekstas;

	cout<<"Iveskite teksta: ";

	getline(cin, tekstas);

   
    int i = tekstas.length() - 1; 
    int tbt=tekstas.length();
    
	while(i !=-1 ){
		if(tekstas[i]==' '){
			
			if(tekstas[i-1]==' '){
				--tbt;
				--i;
			continue;
			}
		--tbt;
		}

		--i;
		
		if(tekstas[i]==' '){
		
			break;
		}
	}
	
	int atsakymas = tbt - i -1;
        
    cout <<"Paskutinio zodzio ilgis - " <<atsakymas<<endl;
        
    return 0;
