<html>
<head>   
    <h2>Вариант: Объявление целочисленной константы с инициализацией на языке C/С++</h2>
</head>
<body>
    <p><b><i>Примеры допустимых строк:</b></i></p>

    <p>const int abc = 123; </p>
        <p>constexpr int b= 123; </p>
        <p>const int d = -123; </p>
        <p><b><i>Разработанная грамматика:</b></i></p>    
        <p>const int a = +-123;</p>
<p>1) DEF -> [‘const’|”constexpr”] CONST </p>
<p>2) CONST -> ‘_’ INT</p>
<p>3) INT -> ‘int’ INTREM</p>
<p>4) INTREM -> ‘_’ ID</p>
<p>5) ID ->letter IDREM</p>
<p>6) IDREM -> letter IDREM</p>
<p>7) IDREM -> ‘=’EQUAL</p>
<p>8) EQUAL -> [+ | -] NUMBER</p>
<p>9) NUMBER -> digit NUMBERREM</p>
<p>10) NUMBERREM -> digit NUMBERREM</p>
<p>	11) NUMBERREM -> ;</p>

    
    
</body>
<p><b><i>Классификация грамматики: </b></i>автоматная</p>        
        <p><b><i>Граф конечного автомата: </b></i></p> 
        <img src = "Автомат.jpg" style="width: 700px">   
    <p><b><i>Тестовые примеры:</b></i></p>
<img src = "Автомат.jpg" style="width: 700px"> 
    <img src = "тест1.png" style="width: 700px"/>
    <img src = "тест2.png" style="width: 700px"/>
    <img src = "тест3.png" style="width: 700px"/>
    <img src = "тест4.png" style="width: 700px"/>
    <img src = "тест5.png" style="width: 700px"/>
    <img src = "тест6.png" style="width: 700px"/>

</html>