# points
points
points.js
Реализуйте и экспортируйте следующие функции для работы с точками:

getQuadrant - функция, которая вычисляет квадрант, в котором находится точка. Ниже приведена схема, показывающая номера квадрантов на плоскости.
        +
      2 | 1
        |
+----------------+
        |
      3 | 4
        +
const point = makePoint(1, 5);
getQuadrant(point); // 1
getQuadrant(makePoint(3, -3)); // 4
Если точка не принадлежит ни одному квадранту (т.е., если она лежит хотя бы на одной из осей координат), то функция должна возвращать null:

const point = makePoint(0, 7);
getQuadrant(point); // null
getQuadrant(makePoint(2, 0)); // null
getSymmetricalPoint - функция, возвращающая новую точку, симметричную относительно начала координат. Такая симметричность означает, что меняются знаки у x и y.
getSymmetricalPoint(makePoint(1, 5)); // makePoint(-1, -5)
calculateDistance - функция, вычисляющая расстояние между точками по формуле: d = sqrt((x2−x1)^2+(y2−y1)^2)
calculateDistance(makePoint(-2, -3), makePoint(-4, 4)); // ≈ 7.28
