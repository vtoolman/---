//некоторые задачи из учебника javascript.ru

/*Напишите полифилл для метода remove для старых браузеров.

Вызов elem.remove():

Если у elem нет родителя – ничего не делает.
Если есть – удаляет элемент из родителя.*/

<!DOCTYPE html>
<html>
<head lang="en">
    <meta charset="UTF-8">
    <title>Павел Бельский</title>
</head>
<body>
<div>Это</div>
<div>Все</div>
<div>Элементы DOM</div>

<script>
    Element.prototype.remove = function() {
        if (this.parentNode !== null){
            this.parentNode.removeChild(this);
        }
    }

    var elem = document.body.children[0];

    elem.remove(); // <-- вызов должен удалить элемент
</script>
</body>
</html>




