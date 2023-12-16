- 👋 Hi, I’m @Mekan2003
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
Mekan2003/Mekan2003 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
import math

def calculate_parallelogram_area(side1, side2, angle_degrees):
    angle_radians = math.radians(angle_degrees)
    area = side1 * side2 * math.sin(angle_radians)
    return area

# Основная программа для ввода данных с консоли
for i in range(10):
    valid_input = False
    while not valid_input:
        try:
            side1 = float(input("Введите длину первой стороны параллелограмма: "))
            side2 = float(input("Введите длину второй стороны параллелограмма: "))
            angle = float(input("Введите угол между сторонами (в градусах): "))
            area = calculate_parallelogram_area(side1, side2, angle)
            print(f"Площадь параллелограмма с сторонами {side1} и {side2}, и углом {angle} градусов: {area}")
            valid_input = True
        except ValueError:
            print("Пожалуйста, введите корректное числовое значение.")
