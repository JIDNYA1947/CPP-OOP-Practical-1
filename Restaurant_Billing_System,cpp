#include <iostream>
#include <string>
using namespace std;

class Restaurant
{
private:
    int orderNumber;
    string itemName;
    float price;
    int quantity;

public:
   
    Restaurant(int orderNo, string item, float itemPrice, int qty)
    {
        orderNumber = orderNo;
        itemName = item;
        price = itemPrice;
        quantity = qty;

        cout << "\nOrder created successfully!" << endl;
    }

    void calculateBill()
    {
        float total = price * quantity;

        cout << "Total Bill: Rs. " << total << endl;
    }

    void updateQuantity(int qty)
    {
        quantity = qty;

        cout << "Quantity updated successfully!" << endl;
    }

    void display()
    {
        float total = price * quantity;

        cout << "\n--- Order Details ---" << endl;
        cout << "Order Number: " << orderNumber << endl;
        cout << "Item Name: " << itemName << endl;
        cout << "Price: Rs. " << price << endl;
        cout << "Quantity: " << quantity << endl;
        cout << "Total Bill: Rs. " << total << endl;
    }

    ~Restaurant()
    {
        cout << "\nDestructor called. Restaurant object destroyed." << endl;
    }
};

int main()
{
    int orderNumber;
    string itemName;
    float price;
    int quantity;
    int newQuantity;

    cout << "Enter Order Number: ";
    cin >> orderNumber;

    cout << "Enter Item Name: ";
    cin >> itemName;

    cout << "Enter Price: ";
    cin >> price;

    cout << "Enter Quantity: ";
    cin >> quantity;

    Restaurant r1(orderNumber, itemName, price, quantity);

    r1.calculateBill();

    cout << "\nEnter new quantity: ";
    cin >> newQuantity;

    r1.updateQuantity(newQuantity);

    r1.display();

    return 0;
}
