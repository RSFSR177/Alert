#include <iostream>

bool isSquare(int num) {
    if (num < 0) {
        return false;
    }
    int sqrt = static_cast<int>(std::sqrt(num));
    return sqrt * sqrt == num;
}

int main() {
    int number = 16;
    if (isSquare(number)) {
        std::cout << number << " является квадратом." << std::endl;
    } else {
        std::cout << number << " не является квадратом." << std::endl;
    }
    return 0;
}
