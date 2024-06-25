#include <iostream>
#include <cmath>

using namespace std;

int main() {
    double x;
    cout << "Введите значение x: ";
    cin >> x;

    // Вычисление всех составляющих функции
    double log2_x = log2(x);
    double sin_x = sin(x);
    double cos_x = cos(x);
    double cos_x2 = cos(x * x);
    double denominator = 1 / (sin_x * sin_x) + 2 - sin(cos_x2);

    // Вычисление значения функции y
    double y = -0.5 + atan(log2_x / denominator);

    // Вывод результата
    cout << "Значение функции y при x = " << x << " равно: " << y << endl;

    return 0;
}
