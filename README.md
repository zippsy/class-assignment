#include<iostream>
using namespace std;

// Class to store pictures 
class dir{
public:
//Data
int Ndir;
int Sdir;
int Edir;
int Wdir;
//Constructor
dir () {
Ndir = Sdir = Edir = Wdir = 45;
}
void display(){
cout <<"North = " << Ndir << endl <<"South = " << Sdir << endl <<"East = " << Edir << endl << "West = " << Wdir << endl;
}
};

class pic{
	public: 
	// Data 
	int rRGB;
	int gRGB;
	int bRGB;
        dir dir1;  
	// Functions

	// Constructor
	pic(){
		rRGB = gRGB = bRGB = 6;
	}

	// Adds some increment to all the RGB values	
	void add(int increment){
		rRGB = rRGB + increment;
		gRGB = gRGB + increment;
		bRGB = bRGB + increment;
	}

	void display(){
	cout << "Red : " << rRGB << endl << "Green : " << gRGB << endl << "Blue : " << bRGB << endl;
	dir1.display();}
};

int main(){
	// int a;
	pic pic1; // pic1 is an object of pic
	pic pic2;
	pic pic3;
	pic1.display();
	//cout << "Enter something : ";
	//cin >> 
	pic1.add(4);
	pic2.add(5);
	pic1.display();
	pic2.display();
	return 0;
}s
