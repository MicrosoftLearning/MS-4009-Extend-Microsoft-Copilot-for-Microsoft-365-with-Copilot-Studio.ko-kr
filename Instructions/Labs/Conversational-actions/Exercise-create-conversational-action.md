# 연습:대화형 작업 만들기

이 연습에서는 "Project ABC"라는 가상의 조직 프로젝트에 대한 정보를 제공하는 대화형 작업을 만들어 보겠습니다.

연습 작업:

- Copilot Studio에서 대화형 작업 만들기
- Microsoft Copilot에 대화형 작업 게시
- Microsoft Copilot에서 대화형 작업 테스트

## 작업 1: (선택 사항) 기본 환경 테스트

먼저 Microsoft 365 Copilot에서 Project ABC에 대해 질문합니다.

1. **Microsoft Teams**를 열고 회사 또는 학교 계정으로 로그인합니다.

1. 사이드바에서 **채팅**을 선택합니다.

1. 채팅 메뉴에서 **Copilot**을 선택합니다.

1. 메시지 작성 상자에 `Who should I contact for questions about Project ABC?`(이)라고 입력합니다. 

1. Microsoft 365 Copilot에는 현재 Project ABC에 대한 정보가 없다는 것을 확인할 수 있습니다.

## 작업 2: 새 대화형 작업 만들기

먼저 Microsoft Copilot에서 새 대화형 작업의 이름, 솔루션, 스키마를 구성합니다.

1. 웹 브라우저에서 [Copilot Studio](https://copilotstudio.microsoft.com)로 이동하고, 메시지가 표시되면 회사 또는 학교 계정으로 로그인합니다.  **건너뛰기**를 선택하여 환영 메시지를 건너뜁니다.

    **참고:** Copilot Studio를 처음 열면 첫 번째 Copilot을 만들기 위한 채팅 인터페이스가 표시될 수 있습니다. 이 경우 오른쪽 위 **...** 메뉴(**만들기** 버튼 옆)를 선택하고 **Copilot 만들기 취소**를 선택한 뒤 **나가기**를 선택하여 채팅 인터페이스를 나가서 Copilot Studio 홈페이지를 봅니다.
1. 왼쪽 탐색 영역에서 **라이브러리**를 선택합니다. 여기서는 기존 작업 및 커넥터 목록을 보고 새로 만들 수 있습니다.
1. 맨 위에 있는 **항목 추가**를 선택합니다.  메뉴에 Microsoft 365용 Copilot 확장 옵션 2가지가 나열됩니다.
:::image type="content" source="../Media/extend copilot options.png" alt-text="창에 Copilot 만들기 또는 작업 만들기라는 Copilot 확장 옵션 2가지가 나열됩니다.":::
1. **새 작업**을 선택합니다.

1. **대화형**을 선택하여 대화형 작업을 만듭니다.

1. **이름** 필드에 `Project ABC` 입력 후 기본 솔루션 및 스키마를 수락합니다.

1. 계속하려면 **만들기**를 선택합니다. 새 대화형 작업이 만들어집니다. 몇 초 정도 걸립니다. 완료되면 작업을 계속 구성하기 위해 자동으로 제작 캔버스로 이동합니다.

## 작업 3: 토픽 구성

다음으로 토픽의 이름 및 트리거를 구성합니다.

1. 대화형 작업 작성 창에서 **토픽** 탭으로 이동합니다.

1. 창 맨 위에 있는 **토픽 이름** 텍스트 상자(기본 이름은 `"Untitled"`)를 선택하고 토픽 이름으로 `Project ABC info`를 입력합니다.

1. 토픽 내의 **트리거** 노드에서 "토픽이 수행하는 작업 설명" 텍스트 아래의 텍스트 상자를 선택한 다음 `Answers questions and provides information about Project ABC, including questions about objectives, points of contact, and rollout timeline.`(이)라고 입력합니다.

## 작업 4: 메시지 보내기

다음으로는 토픽에 노드를 추가하여 Project ABC에 대한 메시지를 보냅니다.

1. 트리거 노드 아래에서 **+** 아이콘을 선택하여 새 노드를 추가합니다.

1. 표시되는 메뉴에서 **메시지 보내기**를 선택합니다.  새 메시지 노드가 만들어졌습니다.

1. 메시지 노드에서 텍스트 상자를 선택하고 다음 내용을 입력합니다. `Project ABC is an initiative aimed at improving the culture and engagement within the company.  Objectives of the project include improved morale, increased employee survey results, and improved culture ratings.  For more information about Project ABC, contact Devon Torres.` 

1. 제작 캔버스 위에 있는 **저장**을 선택하여 변경 내용을 저장합니다.

## 작업 5: 작업 게시

다음으로는 작업을 Microsoft 365 Copilot에서 사용할 수 있도록 게시합니다.

1. 페이지 맨 위에 있는 **게시**를 선택합니다.

1. **플러그인 게시** 페이지에서 **게시**를 선택합니다.

1. **최신 콘텐츠를 게시하시겠습니까?** 페이지에서 Project ABC Info 플러그인이 사용하도록 설정되어 있음을 확인하고 **게시**를 선택합니다.  게시하는 데 몇 분 정도 걸릴 수 있습니다.  게시가 완료되면 알림이 창 맨 위에 표시됩니다.

## 작업 6: 작업 사용 설정 및 테스트

마지막으로 Microsoft 365 Copilot에서 작업을 테스트합니다.

1. **Microsoft Teams**를 엽니다.

1. 사이드바에서 **채팅**을 선택합니다.

1. 채팅 메뉴에서 **Copilot**을 선택합니다.

1. 메시지 작성 영역에서 **Copilot 응답 관리** 버튼을 선택합니다.

1. 플라이아웃에서 **Copilot Studio**를 검색하고 **추가**를 선택하여 Copilot Studio를 추가합니다.
 
2. 이제 **Project ABC info** 작업이 플라이아웃에 나열됩니다.  **Project ABC info**를 사용하도록 설정했음을 확인한 다음 플라이아웃을 닫습니다.

:::image type="content" source="../Media/projectABCInfo-action-enabled.png" alt-text="Teams의 "Copilot 응답 관리" 플라이아웃에 나열된 Project ABC Info 작업의 스크린샷."Manage Copilot response" flyout in Teams.":::

3. 메시지 작성 상자에 `Who should I contact for questions about Project ABC?`(이)라고 입력합니다. 

4. Microsoft 365 Copilot에서 대화형 작업을 호출하여 Project ABC에 대한 정보를 반환하는 것을 확인합니다.

추가 노드를 사용하여 이 대화형 작업을 사용자 지정하거나 확장할 수 있습니다.  예를 들어 새 **생성형 답변** 노드를 만들고 파일을 업로드하면 작업에서 사용할 수 있는 지식을 확장할 수 있습니다.

**참고:** Copilot에서 작업을 테스트할 때는 다음 사항을 기억하세요.
- Copilot은 항상 답변을 자신의 말투로 다시 씁니다. 이 미리 보기에서는 콘텐츠가 변경되지 않은 상태로 최종 사용자에게 전달되는 것이 불가능합니다.
- 대화형 작업에 대한 설명은 작업이 얼마나 안정적으로 호출되는지에 있어 매우 중요합니다. 설명은 오케스트레이터에게 해당 작업이 강한 분야와 제공할 수 있는 답변을 알려줍니다. 설명을 작성할 때 명확한 산문을 사용하고 최상의 결과를 얻으려면 변경 사항을 실험해 보세요.
- 이 단계를 정확하게 수행해도 Copilot이 매번 예측한 대로의 결과를 반환할 것이 보장되지는 않습니다.  플러그인을 호출할 시점과 결과를 반환하는 방법은 Copilot이 결정합니다.

## (선택 사항) 과제: 직접 만들어 보세요!

학습한 내용을 적용하여 원하는 시나리오에 적합한 새 대화형 작업을 만들고 게시하고 테스트해 보세요.  필요에 따라 이 연습의 단계를 검토하세요.