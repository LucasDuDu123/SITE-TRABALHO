<!-- index.html -->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Meu Site</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="tab" onclick="openTab('tab1')">Aba 1</div>
    <div class="tab" onclick="openTab('tab2')">Aba 2</div>

    <div id="tab1Content" class="tab-content">
        <p>Conteúdo da Aba 1</p>
    </div>

    <div id="tab2Content" class="tab-content">
        <p>Conteúdo da Aba 2</p>
    </div>

    <script src="script.js"></script>
</body>
</html>
// script.js
function openTab(tabName) {
    var i, tabContent;
    tabContent = document.getElementsByClassName("tab-content");
    for (i = 0; i < tabContent.length; i++) {
        tabContent[i].style.display = "none";
    }
    document.getElementById(tabName + "Content").style.display = "block";
}
git add .
git commit -m "Adicionando arquivos iniciais"
git push origin master
