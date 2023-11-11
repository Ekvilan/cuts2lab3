<h1 align= "center"> МИНИСТЕРСТВО НАУКИ И ВЫСШЕГО ОБРАЗОВАНИЯ РОССИЙСКОЙ ФЕДЕРАЦИИ ФЕДЕРАЛЬНОЕ ГОСУДАРСТВЕННОЕ БЮДЖЕТНОЕ ОБРАЗОВАТЕЛЬНОЕ УЧРЕЖДЕНИЕ ВЫСШЕГО ОБРАЗОВАНИЯ «САХАЛИНСКИЙ ГОСУДАРСТВЕННЫЙ УНИВЕРСИТЕТ»</h1>
<br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br>
<p align= "center">Лабораторная работа №3</p><br><br><br><br><br><br><br><br>
<p align= "right">Выполнил: Акимов И.В.</p><br><br><br><br><br><br><br><br>
<p align="center">г. Южно-Сахалинск <br> 2023 год</p><br><br><br><br><br><br><br><br>
<h2 style="text-align: center">Введение</h2>
<p align="justify">JavaScript ("JS" для краткости) — это полноценный динамический язык программирования, который применяется к HTML документу, и может обеспечить динамическую интерактивность на веб-сайтах. Его разработал Brendan Eich, сооснователь проекта Mozilla, Mozilla Foundation и Mozilla Corporation. JavaScript сам по себе довольно компактный, но очень гибкий. Разработчиками написано большое количество инструментов поверх основного языка JavaScript, которые разблокируют огромное количество дополнительных функций с очень небольшим усилием. JavaScript невероятно универсален и дружелюбен к новичкам. Обладая большим опытом, вы сможете создавать игры, анимированную 2D и 3D графику, полномасштабные приложения с базами данных и многое другое!</p>
<h2 style="text-align: center">Цели и задачи</h2>
<ol align="justify"> <br>
<h2 align="center">Цели и задачи</h2>
Задачи:
<code>
1. Что выведет код ниже?
alert( null || 2 || undefined );1
2.Что выведет код ниже?
alert( alert(1) || 2 || alert(3) );
3. Что выведет код ниже?
alert( 1 && null && 2 );
4. Что выведет alert (И)?
alert( alert(1) && alert(2) );
5. Что выведет этот код?
alert( null || 2 && 3 || 4 );
6. Напишите условие if для проверки, что переменная age находится в диапазоне между 14 и 90 включительно. «Включительно» означает, что значение переменной age может быть равно 14 или 90.
7.Напишите условие if для проверки, что значение переменной age НЕ находится в диапазоне 14 и 90 включительно. Напишите два варианта: первый с использованием оператора НЕ !, второй – без этого оператора.
8. Какие из перечисленных ниже alert выполнятся?
Какие конкретно значения будут результатами выражений в условиях if(...)?
if (-1 || 0) alert( 'first' );
if (-1 && 0) alert( 'second' );
if (null || -1 && 1) alert( 'third' );
9. Проверка логина
важность: 3
Напишите код, который будет спрашивать логин с помощью prompt.
Если посетитель вводит «Админ», то prompt запрашивает пароль, если ничего не введено или нажата клавиша Esc – показать «Отменено», в противном случае отобразить «Я вас не знаю».
Пароль проверять так:
Если введён пароль «Я главный», то выводить «Здравствуйте!»,
Иначе – «Неверный пароль»,
При отмене – «Отменено».
Блок-схема:
Для решения используйте вложенные блоки if. Обращайте внимание на стиль и читаемость кода.
Подсказка: передача пустого ввода в приглашение prompt возвращает пустую строку ''. Нажатие клавиши Esc во время запроса возвращает null.
10. Какое последнее значение выведет этот код? Почему?
let i = 3;
while (i) {
alert( i-- );
}
11. Для каждого цикла запишите, какие значения он выведет. Потом сравните с ответом.
Оба цикла выводят alert с одинаковыми значениями или нет?
Префиксный вариант ++i:
let i = 0;
while (++i < 5) alert( i );
Постфиксный вариант i++
let i = 0;
while (i++ < 5) alert( i );
12. Для каждого цикла запишите, какие значения он выведет. Потом сравните с ответом. Оба цикла выведут alert с одинаковыми значениями или нет?
Постфиксная форма:
for (let i = 0; i < 5; i++) alert( i );
Префиксная форма:
for (let i = 0; i < 5; ++i) alert( i );
13. При помощи цикла for выведите чётные числа от 2 до 10.
14. Перепишите код, заменив цикл for на while, без изменения поведения цикла.
for (let i = 0; i < 3; i++) {
alert( `number ${i}!` );
}
15. Напишите цикл, который предлагает prompt ввести число, большее 100. Если посетитель ввёл другое число – попросить ввести ещё раз, и так далее. Цикл должен спрашивать число пока либо посетитель не введёт число, большее 100, либо не нажмёт кнопку Отмена (ESC). Предполагается, что посетитель вводит только числа. Предусматривать обработку нечисловых строк в этой задаче необязательно.
16. Натуральное число, большее 1, называется простым, если оно ни на что не делится, кроме себя и 1. Другими словами, n > 1 – простое, если при его делении на любое число кроме 1 и n есть остаток. Например, 5 — это простое число, оно не может быть разделено без остатка на 2, 3 и 4. Напишите код, который выводит все простые числа из интервала от 2 до n. Для n = 10 результат должен быть 2,3,5,7.
17. Напишите if..else, соответствующий следующему switch:
switch (browser) {
  case 'Edge':
    alert( "You've got the Edge!" );
    break;
  case 'Chrome':
  case 'Firefox':
  case 'Safari':
  case 'Opera':
    alert( 'Okay we support these browsers too' );
    break;
  default:
    alert( 'We hope that this page looks ok!' );
}
18. Перепишите код с использованием одной конструкции switch:
 const number = +prompt('Введите число между 0 и 3', '');
if (number === 0) {
  alert('Вы ввели число 0');
}
if (number === 1) {
  alert('Вы ввели число 1');
}
if (number === 2 || number === 3) {
  alert('Вы ввели число 2, а может и 3');
}
19. Следующая функция возвращает true, если параметр age больше 18. В ином случае она запрашивает подтверждение через confirm и возвращает его результат:
function checkAge(age) {
  if (age > 18) {
    return true;
  } else {
    // ...
    return confirm('Родители разрешили?');
  }
}
Будет ли эта функция работать как-то иначе, если убрать else?
function checkAge(age) {
  if (age > 18) {
    return true;
  }
  // ...
  return confirm('Родители разрешили?');
}
Есть ли хоть одно отличие в поведении этого варианта?
20. Следующая функция возвращает true, если параметр age больше 18. В ином случае она задаёт вопрос confirm и возвращает его результат.
function checkAge(age) {
  if (age > 18) {
    return true;
  } else {
    return confirm('Родители разрешили?');
  }
}
Перепишите функцию, чтобы она делала то же самое, но без if, в одну строку.
Сделайте два варианта функции checkAge:
Используя оператор ?
Используя оператор ||
21. Напишите функцию min(a,b), которая возвращает меньшее из чисел a и b.
Пример вызовов:
min(2, 5) == 2
min(3, -1) == -1
min(1, 1) == 1
22. Напишите функцию pow(x,n), которая возвращает x в степени n. Иначе говоря, умножает x на себя n раз и возвращает результат.
pow(3, 2) = 3 * 3 = 9
pow(3, 3) = 3 * 3 * 3 = 27
pow(1, 100) = 1 * 1 * ...* 1 = 1
Создайте страницу, которая запрашивает x и n, а затем выводит результат pow(x,n).
----------------------------------------------------
function func1() {
    alert( null || 2 || undefined );1
}

function func2() {
    alert( alert(1) || 2 || alert(3) );
}

function func3() {
    alert( 1 && null && 2 );
}

function func4() {
    alert( alert(1) && alert(2) );
}

function func5() {
    alert( null || 2 && 3 || 4 );
}

function func6() {
let age = 10;
if (age >= 14 && age <= 90) {
    alert( "В диопазоне" );
    } else {
    alert( "не В диопазоне" );    
    }
}


function func7() {
    let age = 30;
    if (!(age >= 14 && age <= 90)) {
    alert("не В диапазоне");
    } else {
    alert(" В диапазоне");
    }
}

function func8() {
    if (null || -1 && 1) alert( 'third' );
    }


function func9() {

let login = prompt("Введите логин", "");
if (login === "Админ") {
let password = prompt("Введите пароль", "");

if (password === "Я главный") {
alert("Здравствуйте!");
} else if (password === null || password === "") {
alert("Отменено");
} else {
alert("Неверный пароль");
}
} else if (login === null || login === "") {
alert("Отменено");
} else {
alert("Я вас не знаю");
}
}


function func10() {
let i = 3;
while (i) {
  alert( i-- );
}
}


function func11() {
    let i = 0;
    while (i++ < 5) alert( i ); //5
   
    }

    function func12() {
for (let i = 0; i < 5; i++) alert( i ); //0-5

for (let i = 0; i < 5; ++i) alert( i ); //0-4
    }
    
    function func13() {
        for (let i = 2; i <= 10; i += 2) {
           alert(i);
            }
       }


function func14() {
let i = 0;
while (i < 3) {
alert(`number ${i}!`);
i++;
}
}

function func15() {
let number;
do {
number = prompt("Введите число, большее 100", "");
} while (number <= 100 && number !== null);
if (number !== null) {
    alert("Вы ввели число больше 100");
} else {
    alert("Операция отменена");
}
}
function func16() {
    //проверка на простое число
function qqq(num) {
    for(let i = 2, sqrt = Math.sqrt(num); i <= sqrt; i++) {
      if(num % i === 0) {
        return false;
      }
    }
    return num > 1;
  }
  
  function sss(n) {
    const primes = [];
    
    for(let i = 2; i <= n; i++) {
      if(qqq(i)) {
        primes.push(i);
      }
    }
    
    return primes;
  }
  const n = 10;
  const result = sss(n);
  alert(result);
}
    
function func17() {
    let browser = 'Edge';
if (browser === 'Edge') {
    alert("You've got the Edge!");
    } else if (browser === 'Chrome' || browser === 'Firefox' || browser === 'Safari' || browser === 'Opera') {
    alert('Okay we support these browsers too');
    } else {
    alert('We hope that this page looks ok!');
    }
}

function func18() {
const number = +prompt('Введите число между 0 и 3', '');

switch (number) {
case 0:
alert('Вы ввели число 0');
break;
case 1:
alert('Вы ввели число 1');
break;
case 2:
case 3:
alert('Вы ввели число 2, а может и 3');
break;
}
}
function func19() {
    let age=20;
function checkAge(age) {
    if (age > 18) {
      return true;
    }//else {
    // ...
    return confirm('Родители разрешили?');
  //}
}
  alert(checkAge(age));
}

function func20() {
    let age=10;
function checkAge1(age) {
return age > 18 ? true : confirm('Родители разрешили?');
    }
function checkAge2(age) {
return age > 18 || confirm('Родители разрешили?');
}
alert(checkAge1(age));
alert(checkAge2(age));
}

function func21() {
function min(a, b) {
    if (a < b) {
    return a;
    } else {
    return b;
    }
    }
    alert(min(2, 5)); // Выведет 2
    alert(min(3, -1)); // Выведет -1
    alert(min(1, 1)); // Выведет 1
}

function func22() {
function pow(x, n) {
    let result = 1;
    for (let i = 0; i < n; i++) {
    result *= x;
    }
    return result;
    }
    const x = prompt("Введите число x:");
    const n = prompt("Введите степень n:");
    const result = pow(x, n);
    alert(`Результат: ${result}`);
}

    <h2 style="text-align: center">ВЫВОД</h2>
  JavaScript – это язык программирования, который добавляет интерактивность на ваш веб-сайт (например: игры, отклик при нажатии кнопок или при вводе данных в формы, динамические стили, анимация). Эта статья поможет вам начать работать с этим захватывающим языком и даст вам представление о том, на что он способен.

