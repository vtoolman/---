# ---
//некоторые задачи из учебника javascript.ru


<!DOCTYPE html>
<html>
<head lang="en">
    <meta charset="UTF-8">
    <title></title>
</head>
<script>

    var head = {
        glasses: 1
    };

    var table = {
        pen: 3,
        __proto__: head
    };

    var bed = {
        sheet: 1,
        pillow: 2,
        __proto__: table
    };

    var pockets = {
        money: 2000,
        __proto__: bed
    };

    alert(pockets.pen)
    alert(bed.glasses)
    alert(table.money)

</script>
<body>

</body>
