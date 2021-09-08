#include <iostream>
using namespace std;

class Circle {
    int radius;
public:
    Circle() : radius(10) {}
    ~Circle() {}
    void setRadius(int radius) {this->radius = radius;}
    int getRadius() const {return radius;} // const의 기능
                                           // 1. 해당 멤버 함수에서 멤버 변수의 값을 변경할 수 없다.
                                           // 2. 객체에 대한 상수 포인터가 해당 함수를 호출할 수 있게 해 준다.
                                           // * const 로 정의된 멤버 함수가 없으면 객체에 대해 상수 포인터 선언이 불가능하다.
};

int main() {
    Circle *p = new Circle();
    const Circle *pConstObj = new Circle();
    Circle *const pConstPtr = new Circle();

    cout << "p->radius: " << p->getRadius() << endl;
    cout << "pConstObj->radius: " << pConstObj->getRadius() << endl;
    cout << "pConstPtr->radius: " << pConstPtr->getRadius() << endl;

    p->setRadius(30);
    // pConstObj->setRadius(30);
    pConstPtr->setRadius(30);

    cout << "p->radius: " << p->getRadius() << endl;
    cout << "pConstObj->radius: " << pConstObj->getRadius() << endl;
    cout << "pConstPtr->radius: " << pConstPtr->getRadius() << endl;
    return 0;
}
