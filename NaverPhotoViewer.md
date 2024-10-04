# Naver PC PhotoViewer Interaction
> Year: 2024<br>
Role: Interaction Design<br>
Tool: JavaScript/Css<br>
<br>

### Scope of work
- The blog PC photo viewer interaction involves revamping the old blog PC photo viewer.<br>
  블로그 PC 포토 뷰어 인터랙션은 오래된 블로그 PC 포토뷰어를 개편하는 업무<br><br>
- The viewer, which previously displayed only one image, has been improved to allow users to easily and quickly browse all images used in the post.<br>
  기존 한 장의 이미지만 보여주던 뷰어에서 본문에 사용된 모든 이미지를 쉽고 빠르게 찾아볼 수있는 뷰어로 개선<br><br>
- It is implemented with connected usability and detailed interactions.<br>
  연결성 있는 사용성과 디테일한 인터랙션으로 구현<br><br>

<br><br>
## UI Composition
The UI is composed of the top, middle, and bottom sections, and it is designed to interact organically with the mouse.<br>
UI는 상단, 중단, 하단으로 구성되어 있으며 , 마우스에 유기적으로 반응하는 인터랙션을 목표로 구현
<br><br>
![layout](https://github.com/user-attachments/assets/184399d7-b4ca-49fc-842d-9eb366a9b3a1)


<br><br>
## Interaction List
1. Open and close image list (arrow, list in/out)
2. Image transition (top image transition, bottom thumbnail selection/hover/move, left and right arrows)
3. Image controller tooltip
4. Image size adjustment
5. Share popup in/out

<br><br>

   
### 1.Open and close image list (arrow, list in/out)<br>
Interaction where the list opens and closes on mouse hover and click<br>
HOVER, CLICK시 목록이 열리고 닫히는 인터랙션

#### Case1. Image Count Area
Animates 2px up or down on mouse hover and triggers a rotation animation on click.<br>
마우스 오버시 2px 위로 또는 아래로 애니메이션되고 클릭시 회전 애니메이션 실행
<br>
#### Case2. Image List Area
Triggers a vertical position animation (up and down) when selected.<br>
선택시 위, 아래로 포지션 애니메이션 실행
<br><br>

### 2.Image transition (top image transition, bottom thumbnail selection/hover/move, left and right arrows)<br>
When the mouse hovers over the thumbnail area, the size and position of that area change, and the scrollbar fades in/out. When the thumbnail area is clicked, the image corresponding to that item is displayed in the viewer area
<br>
썸네일 영역에 마우스가 HOVER되면 해당영역은 크기및 위치 변화되며 스크롤 바 페이드인/아웃
썸네일 영역 클릭시 해당 아이템에 해당되는 이미지는 뷰어 영역에 표시되는 인터랙션
<br>
<br>
### Mouse Hover/Selected
 
#### Case1. When the mouse hovers over the thumbnail area, the size of the hovered item increases, and the adjacent items move to the left and right.

썸네일 영역 마우스 오버시 해당 아이템의 크기는 커지며 좌우 아이템들은 좌우로 위치 이동 
<br>

#### Case2. The scrollbar fades in when the mouse hovers over the thumbnail area and fades out when the mouse leaves
스크롤 바는 썸네일 영역에 마우스가 오버되면 페이드 인, 아웃되면 페이드 아웃 애니메이션 실행
<br>

#### Case3.The left and right buttons move horizontally when the mouse hovers over them, reduce in scale when the mouse is pressed down, and return to their original scale when clicked (mouse released)
좌우 버튼은 마우스 오버시 좌우로 포지션 이동, 마우스 다운시 스케일 축소 클릭시(마우스 놓았을때) 스케일 원래대로 돌아감
<br><br>

### 3.Image controller tooltip<br>
The tooltip icon triggers an animation based on mouse events
<br>
툴팁 아이콘은 마우스 이벤트에 따라 애니메이션 실행
<br>
- Mouse Hover
- Mouse Active
<br><br>
### 4.Image size adjustment<br>
Applied animation properties during scale adjustment to enhance detailed interactions
<br>
스케일 조정시 애니메이션 속성 적용해 디테일을 높힌 인터랙션
<br><br>
### 5.Share popup in/out<br>
When the menu icon is hovered over or selected
<br>
메뉴 아이콘 마우스 오버/ 선택 시
<br><br>
