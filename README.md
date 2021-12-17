# Lecture-6-
bool Checker(int num) { bool check = false; if (num > 0) { if ((num % 2) == 0) { check = true; } } return check; } void NumChecker(int num) {

if (Checker(num)) {
	cout << "the number is even" << endl;
}
else
	cout << "the number is odd" << endl;
} int main() {

int num;
cout << "Enter a number: "; cin >> num;

NumChecker(num);

return 0;
}

//Slide 25 (Number Checker) #include using namespace std;

bool Checker(int num) { bool check = false; if (num >= 0) { check = true; } return check; } void NumChecker(int num) {

if (Checker(num)) {
	cout << "the number is positive" << endl;
}
else
	cout << "the number is negative" << endl;
} int main() { int num; cout << "Enter a number: "; cin >> num; NumChecker(num); return 0; }

//Slide 26 (Profit or Loss) #include using namespace std;

void Display() { int netPrice, salePrice, net; cout << "Enter Purchase Price: "; cin >> netPrice; cout << "Enter Sale Price: "; cin >> salePrice; net = netPrice - salePrice; if (net > 0) { cout << "Profit of: " << net << endl; } else cout << "Loss of: " << net << endl; } int main() {

Display();

return 0;
}

//Slide 27 (Name that Shape) #include

using namespace std;

void Display() { int numSides; bool run = true; while (run) { cout << "Enter the numbers of sides: "; cin >> numSides; system("cls"); if (numSides >= 3 && numSides <= 10) { if (numSides == 3) { cout << "it's a triangle" << endl; run = false; } else if (numSides == 4) { cout << "it's a square" << endl; run = false; } else if (numSides == 5) { cout << "it's a pentagon" << endl; run = false; } else if (numSides == 6) { cout << "it's a hexagon" << endl; run = false; } else if (numSides == 7) { cout << "it's a heptagon" << endl; run = false; } else if (numSides == 8) { cout << "it's a octagon" << endl; run = false; } else if (numSides == 9) { cout << "it's a nonagon" << endl; run = false; } else if (numSides == 10) { cout << "it's a decagon" << endl; run = false; } } else cout << "Error. Please try again" << endl; } }

int main() { Display(); return 0; }
