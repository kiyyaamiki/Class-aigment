#include <iostream>
#include <string>
using namespace std;

class Book {
private:
    // Data members (Encapsulation)
    string title;
    string author;
    int pages;

public:
    // Default constructor
    Book() {
        title = "power";
        author = "human being";
        pages = 0;
    }

    // Parameterized constructor
    Book(string t, string a, int p) {
        title = t;
        author = a;
        pages = p;
    }

    // Member function to display book details
    void displayInfo() {
        cout << "Book Title: " << title << endl;
        cout << "Author: " << author << endl;
        cout << "Pages: " << pages << endl;
    }

    // Setter functions (to update data)
    void setTitle(string t) {
        title = t;
    }

    void setAuthor(string a) {
        author = a;
    }

    void setPages(int p) {
        pages = p;
    }

    // Getter functions (to access data)
    string getTitle() {
        return title;
    }

    string getAuthor() {
        return author;
    }

    int getPages() {
        return pages;
    }
};

int main() {
    // Using default constructor
    Book book1;
    book1.displayInfo();
    cout << endl;

    // Updating details using setters
    book1.setTitle("C++ Programming");
    book1.setAuthor("Bjarne Stroustrup");
    book1.setPages(350);
    book1.displayInfo();
    cout << endl;

    // Using parameterized constructor
    Book book2("1984", "George Orwell", 328);
    book2.displayInfo();

    return 0;
https://youtu.be/iM48VDuPRQk?si=8CEGQuQwJfQRl6JX
