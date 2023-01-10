# Tabmenu

function setMenu(value) {
  if (value == 'tab1') {
    document.getElementById('web').style.display = 'block'; 
    document.getElementById('native').style.display = 'none'; 
    document.getElementById('sw').style.display = 'none'; 
  }

  if (value == 'tab2') {
    document.getElementById('web').style.display = 'none'; 
    document.getElementById('native').style.display = 'block'; 
    document.getElementById('sw').style.display = 'none'; 
  }

  if (value == 'tab3') {
    document.getElementById('web').style.display = 'none'; 
    document.getElementById('native').style.display = 'none'; 
    document.getElementById('sw').style.display = 'block'; 
  }

}

클릭시마다 css에 입력된 디스플레이 속성을 다 바
