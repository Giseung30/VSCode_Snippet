# 🚀 VS Code Snippets
> 개발 생산성을 높이기 위한 VS Code 코드 스니펫( Snippets) 모음입니다.

## 🛠️ 스니펫 생성 및 적용 방법 (How to Use)
> 스니펫을 **VS Code**에 적용하는 방법입니다.

### 1. 스니펫 설정창 열기
+ `File` > `Preferences` > `Configure Snippets` 선택

### 2. 언어 선택
+ 스니펫을 적용할 언어를 선택하거나, 모든 언어에서 공통으로 사용하려면 `New Global Snippets file...`을 선택합니다.

### 3. 코드 작성 (JSON)
+ 설정 파일 내에 아래와 같은 형식으로 스니펫을 추가합니다.
```JSON
{
  "sfor": {
    "prefix": "sfor",
    "body": [
      "for (let ${1:i} = 0, ${2:l} = ${3:0}; $1 < $2; ++$1) {",
      "    $4",
      "}"
    ],
    "description": "for문을 만듭니다"
  }
}
```
### 4. 주요 속성 설명
<table style="width:100%">
    <thead>
        <tr>
            <th>구성 요소</th>
            <th>상세 설명</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td><strong>prefix</strong></td>
            <td>코드를 불러올 <b>단축어</b>입니다. (예: sfor 입력 시 스니펫 호출)</td>
        </tr>
        <tr>
            <td><strong>body</strong></td>
            <td>실제로 입력될 <b>코드 내용</b>입니다. 한 줄씩 배열 형태로 작성합니다.</td>
        </tr>
        <tr>
            <td><strong>$1, $2, ...</strong></td>
            <td><b>Tab</b> 키를 눌렀을 때 커서가 이동할 순서입니다. (Shift + Tab으로 이전 이동 가능)</td>
        </tr>
        <tr>
            <td><strong>${1:(기본값)}</strong></td>
            <td>커서 이동 시 <b>기본값</b>을 미리 지정할 수 있습니다. (예: i, l 등)</td>
        </tr>
        <tr>
            <td><strong>description</strong></td>
            <td>해당 스니펫에 대한 <b>설명문</b>입니다.</td>
        </tr>
    </tbody>
</table>

## 📂 저장소 구조
본 레포지토리는 언어별로 스니펫 파일을 관리합니다
+ `/javascript.json` - 자바스크립트(JavaScript)

## 🔗 Reference
+ [[VS Code] 코딩 속도를 높이는 기술, 코드 스니펫(Code Snippet)](https://giseung.tistory.com/89)