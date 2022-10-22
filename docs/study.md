# 공부내용 정리

## 01. Asset

1. /asset/img 경로에 사용할 이미지를 추가한다.
2. /pubspec.yaml 파일에서 flutter 섹션 하위에 값을 추가해준다.
3. assets 안에 asset/img/ 작성하고 flutter pub get 명령어를 입력한다. ( 버튼 클릭 )

## 02. Stateless 사용해보기

1. 외워야 하는 구조
    1. lib/main.dart 안에 void main() 함수가 있어야 한다.
    2. void main() 함수안에는 runApp()가 있어야 앱이 구동된다.
    3. runApp() 안에는 어떤 유형의 앱을 사용할지 결정해야 하는데 현재는 MaterialApp() 이다.
    4. MaterialApp 에서 home 인자에 Scaffold 를 주입한다. ( 앱바 설정 등의 최상위 트리에서 필요한 기능들이 구현되어 있음)
    5. Scaffold() 안에 body 인자에 개발에 필요한 각종 위젯들을 사용하면 된다!
2. StatelessWidget을 상속받는 HomeScreen 클래스 생성
    1. 필수적으로 Widget build() 메서드를 오버라이드해야 한다.
    2. MaterialApp의 home이 변경될 때는 핫리로드가 적용되지 않고 build 메서드 안의 값만 핫 리로드가 적용된다.

## 03. Column 사용해보기
1. Center 위젯은 child 파라미터에 위젯 하나를 넣기 때문에 이미지 위젯 하나만 보여줄 수 있었다. 다른 위젯이 필요하다.
2. 이런 경우에 사용할 수 있는 위젯이 Column(세로), Row(가로) 위젯인데 현재 필요한건 세로로 쌓을 수 있는 Column 위젯이 필요하다.
3. Column 위젯은 가장 위에 children 위젯들을 차례대로 배치하는게 기본 룰 변경하고 싶음.
4. mainAxisAlignment 속성으로 배치가 가능함.
   1. mainAxis: 주축(세로)
   2. Alignment : 정렬
5. 가운데 정렬하고 싶어! mainAxisAlignment: MainAxisAlignment.center, 파라미터 사용 세로 가운데로 정렬 됨
## 편의 단축키

1. 옵션 + 엔터 기능으로 힌트를 통한 코드 자동 생성 및 위젯 래핑 기능 등을 사용할 수 있다. **
2. 커맨드 + 옵션 + l 버튼으로 코드 정리를 할 수 있으며

