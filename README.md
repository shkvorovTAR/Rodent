# Rodent
https://github.com/Anaga/TARvg17/tree/master/OopRodent
TARgv17 Homework: oopRodent

main class for all rodents.

C++ Inheritance https://www.tutorialspoint.com/cplusplus/cpp_inheritance.htm

C++ Class Constructor and Destructor https://www.tutorialspoint.com/cplusplus/cpp_constructor_destructor.htm

class Rodent
{
    double weight =1.0; //gramm
    int age=0; //age in days
    int maxLifeSpan = 1000; // in days
    QString name;
public:
    Rodent(QString name); // Constructor
   ~Rodent(); // Destructor
    QString getName() {return name;}
    void feed(double food); // Feed rodent with some gramm of food
    bool lifeDay(); // spend one day of life, ferurn false is rodent die.
};

class Mouse: public Rodent{
public:
    Mouse(QString name); // Constructor
    void addTwoGrams();   // super power :)
    bool lifeDay();     // function overloading
};

В задании Rodent class доделать производный класс, чтобы у нас были и мышки, и хомячки.
У каждого есть базовые методы - прожить один день, поесть, и какие то особые, только им присущие методы (Супер сила :) )
Питание - грызун не способен скушать больше чем 50% от своего веса в день.
У каждого вида есть свой предел времени жизни, и при превишении его, есть шанс 50/50 что грызун умрет от старости.
Супер способности у Мышек - добавить 2 грама просто так
Супер способности у Хомяков - прожить 2 дня просто так
И написать тестовую программу, которая преверять, скольок кто живет, если нормально кушать, и вообще, иногда использовать супер способности. 
