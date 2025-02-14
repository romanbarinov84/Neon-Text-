# 🌟 Neon Text Effect  
**Neon Text Effect** — это анимация бегущего текста с неоновыми цветами, реализованная с помощью JavaScript и CSS.  

## 🚀 Демо  
Посмотреть [https://romanbarinov84.github.io/Neon-Text-/]

## 📌 Функциональность  
- Текст отображается по буквам с анимацией  
- Цвет каждой буквы меняется случайно каждые 500 мс  
- Используется `hsl()` для создания ярких цветов

- # 📁 Структура проекта
 ├── index.html       # Основной HTML-файл
 ├── style.css        # Стили оформления
 ├── main.js          # Скрипт анимации
 ├── README.md        # Описание проекта

 # 📜 Код
## Пример основного кода:

### const $textContent = document.getElementById("text");

### const innerText = "Created Your Style Neon Text"

 for(let i = 0; i < innerText.length; i++){
 
     let $spanText = document.createElement("span");
     
   $spanText.classList.add("letter");
   
   $spanText.innerHTML = innerText[i];
   
   $textContent.appendChild($spanText);
}

function addNeonText() {
let $letters = document.querySelectorAll(".letter");

for(let i = 0; i < $letters.length; i++){
    
$letters[i].style.color = `hsl(${Math.random() * 360}, 100% , 70%)`
     
        
    }
}

setInterval(addNeonText, 500)

✨ Создано с ❤️ для экспериментов с анимацией! 🚀
