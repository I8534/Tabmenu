# Tabmenu




ㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡ

자바스크립트

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

클릭시마다 css에 입력된 디스플레이 속성을 다 바꿔주는 것이다.


저기서 value는 매개변수이다.

html에서 마크업이 이렇게 되어있다.

    <div class="tab-box-list">
      <div class="tab-box-item" onclick="setMenu('tab1')">웹 개발</div>
      <div class="tab-box-item" onclick="setMenu('tab2')">네이티브앱 개발</div>
      <div class="tab-box-item" onclick="setMenu('tab3')">응용 sw 개발</div>
    </div>

onclick="setMenu('tab1') 즉, 온클릭시 세트메뉴 함수가 작동하는 것인데 정확히는 세트메뉴 중 탭1이 작동하도록 하는 것이다.

근데 여기서 자바스크립트에서 함수에 매개변수를 value라고 입력함으로서 매개 즉 중개하는 놈을 탭1 탭2 탭3라고 입력함으로서

선택할 수 있게 하는 것이다.

