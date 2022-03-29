
## Cпособы обьявления переменных JavaScript:

 - В новом стандарте JavaScript ES2015 переменные обьявляют с помощью двух ключевых слов : 'let' или  'const'.

- Ключевое слово 'var' является устаревшим и не применяется в новом стандарте.

 - Ключевое слово 'let' применяется тогда ,когда значение переменной в последующем коде будет изменяться.

- Eсли значение нужно сделать таким ,которое не меняется, то используется ключевое слово 'const'.

- При попытке изменить значение переменной ,обьявленной с помощью ключевого слова 'const' возникает ошибка.

## Разница между 'prompt' и 'confirm':

</hr>

Prompt выводит сообщение и возвращает введенное пользователем в диалоговом окне значение  или null,если ввод отменен.

Confirm выводит диалоговое окно с сообщением, который имеет только два варианта ответа - OK или Cancel и возвращает только два варианта значения-либо 'true'(OK) либо false(Cancel) 

'Сonfirm'   получает от пользователя данные только типа boolean,а 'prompt' получает от пользователя тип данных number,string либо null.

## Неявное преобразование типов:

Так как JavaScript это слабо типизированный язык, преобразование между разными типами может происходить автоматически, и это называется неявным преобразованием типов.


## Пример неявного преобразования:

При сложении, если хотя бы один из операндов имеет тип данных string 

 остальные операнды тоже  приводятся к типу данных string и результат имеет тип данных string:

```js

let randomString = '123';
let randomNumber = 144;

console.log(randomString + randomNumber);

// Результат '123144'- тип данных string

```

</hr>

Остальные операторы приводят все операнды к числовому типу

```js

let randomString = '12';
let randomNumber = 12;

console.log(randomString*randomNumber);

// Результат 144 - тип данных number

```

</hr>

В логических операторах все операнды приводятся к типу boolean:

например:

```js

console.log( 0 || 1 );

// 1 будет приведен к булевому значению true,а 0 -false  

// в консоль будет выведено первое из значений приведенное к true

// Результат: 1

```
</hr>

Условный оператор if (..) {...} автоматически приводит значение в круглых скобках к типу boolean и если значение в круглых скобках приводится  true то выполняется содержимое фигурных скобок.

```js

if(100){

    console.log('one hundred');
}

// 100 приведено к булевому значению true 



```

